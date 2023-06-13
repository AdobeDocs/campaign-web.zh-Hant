---
audience: end-user
title: 設計推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web設計推播通知傳遞
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 7%

---

# 設計推播傳遞 {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="推播 Android 內容"
>abstract="定義推播 Android 內容。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="推播 iOS 內容"
>abstract="定義推播 iOS 內容。"

## 訊息 {#push-message}

>[!BEGINTABS]

>[!TAB Android]

使用Firebase Cloud Messaging，您可以在兩種訊息型別之間進行選擇：

* 此 **[!UICONTROL 資料訊息]e** 由使用者端應用程式處理。 這些訊息會直接傳送至行動應用程式，在裝置上產生和顯示Android通知。 資料訊息僅包含您的自訂應用程式變數。

  若要定義內容、個人化資料及新增動態內容，請按一下 **[!UICONTROL 訊息]** 欄位並使用運算式編輯器。 您可以存取此編輯器來自訂您的訊息，在 **[!UICONTROL 應用程式變數]** 選單中，您的應用程式變數會自動新增。 這些變數可讓您定義通知行為。 例如，您可以設定當使用者啟動通知時顯示的特定應用程式畫面。

  ![](assets/push_content_4.png)

* 此 **[!UICONTROL 通知訊息]**，會由FCM SDK自動處理。 FCM會自動代表使用者端應用程式在使用者裝置上顯示訊息。 通知訊息包含預先定義的一組引數和選項，但仍可使用自訂應用程式變數進一步個人化。

  若要撰寫訊息，請按一下 **[!UICONTROL 標題]** 和 **[!UICONTROL 內文]** 欄位。 使用運算式編輯器來定義內容、個人化資料及新增動態內容。

  若要進一步個人化您的推播通知，您可以選擇要新增至推播通知的影像，通知的圖示可顯示在您的設定檔的裝置上及其顏色。

  ![](assets/push_content_3.png)

>[!TAB iOS]

若要撰寫訊息，請按一下 **[!UICONTROL 標題]** 和 **[!UICONTROL 內文]** 欄位。 使用運算式編輯器來定義內容、個人化資料及新增動態內容。

您可以新增 **[!UICONTROL 字幕]**，iOS通知裝載之字幕引數的值。 請參閱本區段。

靜音推播模式允許將「靜音」通知傳送至行動應用程式。 使用者未意識到通知的到達。 它會直接傳輸到應用程式。

![](assets/push_content_1.png)

>[!ENDTABS]

## 進階設定 {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| 參數 | 說明 |
|---------|---------|
| **[!UICONTROL 音效]** | 設定裝置收到通知時播放的音效。 |
| **[!UICONTROL 通知計數]** | 設定直接在應用程式圖示上顯示的新未讀取資訊數目。 這可讓使用者快速檢視擱置通知的數量。 |
| **[!UICONTROL 管道 ID]** | 設定通知的頻道ID。 在收到任何具有此管道ID的通知之前，應用程式必須建立具有此管道ID的管道。 |
| **[!UICONTROL 點按動作]** | 定義與使用者點按您的通知相關聯的動作。 這會決定使用者與通知互動時的行為，例如開啟特定畫面或在應用程式中執行特定動作。 |
| **[!UICONTROL 標記]** | 設定用來取代通知抽屜中現有通知的識別碼。 這有助於防止累積多個通知，並確保只顯示最新的相關通知。 |
| **[!UICONTROL 優先順序]** | 設定通知的優先順序層級，可以是預設、最低、低或高。 優先順序層級會決定通知的重要性和緊急程度，進而影響其顯示方式以及是否可以略過某些系統設定。 有關詳細資訊，請參閱 [FCM檔案](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL 可見度]** | 設定通知的可見度等級，可為公開、私人或秘密。 可見度等級會決定通知內容在鎖定畫面和其他敏感區域上顯示的比例。 如需詳細資訊，請參閱 [FCM檔案](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL 粘性]** | 啟動後，通知仍可見，即使使用者按一下它。 <br>如果停用，則當使用者與通知互動時，會自動將其關閉。 粘著行為可讓重要通知在熒幕上持續較長時間。 |
| **[!UICONTROL 應用程式變數]** | 允許您定義通知行為。 這些變數可完全自訂，並包含在傳送至行動裝置的訊息裝載中。 |

>[!TAB iOS]

![](assets/push_content_2.png)

| 參數 | 說明 |
|---------|---------|
| **[!UICONTROL 嚴重警報模式]** | 啟用此選項可將聲音新增至您的通知，即使使用者的電話設為焦點模式或iPhone已靜音亦然。 這可確保使用者注意到重要警示。 |
| **[!UICONTROL 清除徽章]** | 啟用此選項以重新整理應用程式圖示上顯示的徽章值。 這可確保徽章準確反映新的未讀取資訊的數量。 |
| **[!UICONTROL 通知計數]** | 設定將直接顯示在應用程式圖示上的數字，指示新的未讀取資訊的數量。 這可提供使用者的快速視覺參考。 |
| **[!UICONTROL 數量]** | 音量從0到100。 |
| **[!UICONTROL 可變內容]** | 啟用此選項可允許行動應用程式下載與通知相關的媒體內容。 有關詳細資訊，請參閱 [Apple 開發人員文件](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)。 |
| **[!UICONTROL 關聯性分數]** | 將相關性分數設定為0到100，以優先處理通知摘要中的通知順序。 分數越高表示通知越重要。 |
| **[!UICONTROL 中斷層級]** | <ul> <li>**[!UICONTROL 作用中]**：根據預設，系統會立即顯示通知、在畫面上點亮，並可播放音效。 通知不會突破焦點模式。</li><li>**[!UICONTROL 被動]**：系統會將通知新增至通知清單，而不會點亮熒幕或播放音效。 通知不會突破焦點模式。</li><li>**[!UICONTROL 時效性]**：系統會立即顯示通知、點亮熒幕、播放聲音並突破焦點模式。 此層級不需要Apple的特殊許可權。</li> <li>**[!UICONTROL 關鍵]**：系統會立即顯示通知、點亮熒幕，並略過靜音切換或聚焦模式。 請注意，此層級需要Apple的特殊許可權。</ul> |
| **[!UICONTROL Thread-id]** | 用於將相關通知分組在一起的識別碼。 具有相同對話串ID的通知會在通知清單中整理為單一對話或對話串。 |
| **[!UICONTROL 類別]** | 指定與通知相關聯的類別ID名稱。 如此可顯示動作按鈕，讓使用者直接從通知執行各種工作，而無需開啟應用程式。 |
| **[!UICONTROL 目標內容 ID]** | 用來在通知開啟時鎖定要轉送的應用程式視窗的識別碼。 |
| **[!UICONTROL 啟動影像]** | 指定當使用者選擇從通知啟動您的應用程式時要顯示的啟動影像檔名稱。 將會顯示選取的影像，而非應用程式的一般啟動畫面。 |
| **[!UICONTROL 應用程式變數]** | 允許您定義通知行為。 這些變數可完全自訂，並包含在傳送至行動裝置的訊息裝載中。 |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



