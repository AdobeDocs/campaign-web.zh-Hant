---
audience: end-user
title: 開始在 Campaign v8 Web 中使用訊息和傳遞
description: 了解如何使用 Campaign Web 處理傳遞和傳送訊息
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 35%

---

# 開始在 Campaign Web 中使用訊息 {#gs-messages}

透過Adobe Campaign，您可以傳送跨頻道行銷活動，包括電子郵件、簡訊和推播通知，並使用各種專用報告來衡量其成效。 這些訊息是透過傳遞進行設計和傳送，而且可針對每位收件者進行個人化。這些傳遞可以是獨立的，或包含在行銷活動內容中。

Adobe Campaign v8 提供下列傳送頻道：

* **電子郵件頻道**：電子郵件傳遞功能可讓您傳送個人化電子郵件給目標群體。瞭解如何在中建立和傳送電子郵件 [此頁面](../email/create-email.md).

* **簡訊頻道**：行動裝置頻道上的傳遞可讓您傳送個人化SMS給目標群體。  瞭解如何在中建立和傳送簡訊 [此頁面](../sms/create-sms.md).

* **行動應用程式頻道**：行動應用程式傳送可讓您傳送通知至 iOS 和 Android 系統。瞭解如何在中建立和傳送推播通知 [此頁面](../push/gs-push.md).

## 建立傳遞

您可以從以下位置建立獨立傳送： **傳遞** 主功能表，或在行銷活動內容中建立傳送。

>[!BEGINTABS]

>[!TAB 建立獨立傳送]

若要建立獨立傳送，請遵循下列步驟：

1. 瀏覽至 **[!UICONTROL 傳遞]** 功能表，然後按一下 **[!UICONTROL 建立傳遞]** 按鈕。
1. 選擇傳遞的管道。 在以下章節中進一步瞭解傳遞管道以及如何定義傳遞內容：

   * [電子郵件通道](../email/create-email.md)
   * [推播通知頻道](../push/gs-push.md)
   * [SMS 頻道](../sms/create-sms.md)

1. 定義主要目標和控制組的傳送對象。 進一步瞭解中的對象 [本節](../audience/about-audiences.md).
1. 定義訊息內容。
1. （選用）定義傳遞排程。 如果未定義排程，則會在按一下 **[!UICONTROL 傳送]** 按鈕。
1. 按一下  **[!UICONTROL 檢閱並傳送]** 按鈕以檢查您的設定。
1. 使用  **[!UICONTROL 模擬內容]** 按鈕以測試您的傳遞和個人化設定。 進一步瞭解中的訊息模擬 [本節](../preview-test/preview-test.md).
1. 按一下  **[!UICONTROL 準備]** 按鈕以計算目標母體並產生訊息。 準備步驟可能需要幾分鐘的時間。 準備完成後，訊息即可傳送。 發生錯誤時，請瀏覽至 **記錄檔** 以檢查警示和警告。
1. 檢查結果，然後按一下  **[!UICONTROL 傳送]** 按鈕以開始傳送訊息。
1. 傳送訊息後，請瀏覽至「報表」區段以存取關鍵量度。 進一步瞭解中的傳遞報告 [本節](../reporting/reports.md).

>[!TAB 在行銷活動中建立傳遞]

若要在行銷活動中建立傳送，請遵循下列步驟：

1. 建立行銷活動或開啟現有的行銷活動。

如需如何設定行銷活動的詳細資訊，

>[!ENDTABS]


## 選擇如何傳送訊息{#gs-send-msg}

當您的訊息建立完成且其內容經過設計和測試後，您就可以選擇要如何傳送。 

Campaign 提供一組功能，可以：

* 手動傳送訊息至主要目標

* 傳送與[行銷活動](../campaigns/gs-campaigns.md)相關的訊息

* 透過[工作流程](../workflows/channel-activities.md)傳送訊息


## 新增個人化{#personalization}

Adobe Campaign傳送的訊息可透過多種方式個人化


## 傳送和追蹤記錄{#gs-tracking-logs}

傳送傳遞後進行監視是確保行銷活動效率並與客戶溝通的關鍵步驟。 您可以在傳送傳遞後進行監視，並瞭解傳送失敗和隔離的管理方式。
