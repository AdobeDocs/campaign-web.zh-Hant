---
audience: end-user
title: 設計推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web設計推播通知傳遞
badge: label="Alpha" type="Positive"
source-git-commit: 965c2d72d81233c98beb4e4bc3c76692c7bf3990
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 7%

---

# 設計推播傳遞 {#content-push}

## 訊息 {#push-message}

>[!BEGINTABS]

>[!TAB Android]

使用Firebase Cloud Messaging，您可以在兩種訊息型別之間進行選擇：

* 此 **資料訊息**，由使用者端應用程式處理。 訊息會直接傳送至行動應用程式，以產生Android通知並顯示至裝置。 資料訊息僅包含您的自訂應用程式變數。

   按一下 **[!UICONTROL 訊息]** 欄位並使用運算式編輯器來定義內容、個人化資料及新增動態內容。

* 通知訊息，由FCM SDK自動處理。 FCM會自動代表使用者端應用程式在使用者裝置上顯示訊息。 通知訊息包含預先定義的一組引數和選項，但仍可使用自訂應用程式變數進一步個人化。

   若要撰寫訊息，請按一下 **[!UICONTROL 標題]** 和 **[!UICONTROL 內文]** 欄位。 使用運算式編輯器來定義內容、個人化資料及新增動態內容。

   若要進一步個人化您的推播通知，您可以選擇要新增至推播通知的影像，通知的圖示可顯示在您的設定檔的裝置上及其顏色。

>[!TAB iOS]

若要撰寫訊息，請按一下 **[!UICONTROL 標題]** 和 **[!UICONTROL 內文]** 欄位。 使用運算式編輯器來定義內容、個人化資料及新增動態內容。

您可以新增 **[!UICONTROL 字幕]**，iOS通知裝載之字幕引數的值。 請參閱本區段。

靜音推播模式允許將「靜音」通知傳送至行動應用程式。 使用者未意識到通知的到達。 它會直接傳輸到應用程式。

>[!ENDTABS]

## 進階設定 {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL 音效]**：設定裝置收到通知時播放的聲音。

* **[!UICONTROL 通知計數]**：設定新未讀取資訊的數量，以直接在應用程式圖示上顯示。

* **[!UICONTROL 管道ID]**：設定通知的頻道ID。 在收到任何具有此管道ID的通知之前，應用程式必須建立具有此管道ID的管道。

* **[!UICONTROL 點按動作]**：設定與使用者點按您的通知相關聯的動作。

* **[!UICONTROL 標籤]**：設定用來取代通知抽屜中現有通知的識別碼。

* **[!UICONTROL 優先順序]**：將通知的優先順序層級設定為預設、最低、低或高。 如需詳細資訊，請參閱FCM檔案。

* **[!UICONTROL 可見度]**：將通知的可見度等級設定為公開、私人或秘密。 如需詳細資訊，請參閱FCM檔案。

* **[!UICONTROL 粘性]**：如果已停用，使用者點按通知時會自動將其取消。 如果啟用，即使使用者按一下通知，仍會顯示通知。

>[!TAB iOS]

* **[!UICONTROL 嚴重警示模式]**：啟用此選項，即使使用者的手機設定為焦點模式或iPhone設為靜音，也可以將聲音新增到您的通知中。

* **[!UICONTROL 清除徽章]**：啟用此選項以重新整理徽章值。

* **[!UICONTROL 通知計數]**：設定將用於直接在應用程式圖示上顯示的新未讀取資訊數量。

* **[!UICONTROL 音量]**：音量從0到100。

* **[!UICONTROL 可變內容]** (僅限iOS)：在推播裝載中傳送可變內容旗標，並允許推播通知內容由iOS SDK中提供的通知服務應用程式擴充功能修改。 有關詳細資訊，請參閱 [Apple 開發人員文件](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)。啟用此選項可允許行動應用程式下載媒體內容。

* **[!UICONTROL 關聯性分數]**：將關聯性分數設定為0到100。 系統會使用此選項來排序通知摘要中的通知。

* **[!UICONTROL 中斷層級]**:

   * **[!UICONTROL 作用中]**：根據預設，系統會立即顯示通知、在畫面上點亮，並可播放音效。 通知不會突破焦點模式。

   * **[!UICONTROL 被動]**：系統會將通知新增至通知清單，而不會點亮熒幕或播放音效。 通知不會突破焦點模式。

   * **[!UICONTROL 時效性]**：系統會立即顯示通知、點亮熒幕、播放聲音並突破焦點模式。 此層級不需要Apple的特殊許可權。

   * **[!UICONTROL 關鍵]**：系統會立即顯示通知、點亮熒幕，並略過靜音切換或聚焦模式。 請注意，此層級需要Apple的特殊許可權。

* **[!UICONTROL Thread-id]**：用於將相關通知分組在一起的識別碼。

* **[!UICONTROL 類別]**：將顯示動作按鈕的類別ID名稱。 這些通知可讓使用者以更快的方式回應通知，執行不同的工作，而不需在應用程式中開啟或導覽。

* **[!UICONTROL 目標內容ID]**：用來在通知開啟時鎖定要轉送的應用程式視窗的識別碼。

* **[!UICONTROL 啟動影像]**：要顯示的啟動影像檔名稱。 如果使用者選擇啟動您的應用程式，則會顯示選取的影像，而非您的應用程式啟動畫面。

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



