---
product: campaign
title: 使用傳遞
description: 了解如何在 Campaign Web 中建立您的第一個傳遞
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
source-git-commit: ecff4e56bd346aadf381a1bf2077204804938f62
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 88%

---


# 建立傳遞 {#create-delivery}

您可以從「**[!UICONTROL 傳遞]**」左側選單建立獨立的傳遞，或在工作流程的內容中建立傳遞，無論是否在行銷活動之內。

瀏覽下面的標籤以了解如何建立傳遞：

>[!BEGINTABS]

>[!TAB 建立獨立傳遞]

若要建立獨立傳遞，請依照以下步驟進行：

1. 瀏覽至左側導覽上的「**[!UICONTROL 傳遞]**」選單，然後按一下「**[!UICONTROL 建立傳遞]**」按鈕。

   ![](assets/create-a-delivery.png){zoomable="yes"}

1. 選擇要用於傳遞的管道。
1. 定義主要目標和控制組的傳遞客群。[進一步瞭解對象](../audience/about-recipients.md)。

   ![](assets/select-audience.png){zoomable="yes"}{width="70%" align="left"}

1. 定義訊息內容。若要了解傳遞管道以及如何定義傳遞內容的詳細資訊，請參閱以下章節：

   * [電子郵件管道](../email/create-email.md)
   * [推播通知管道](../push/gs-push.md)
   * [簡訊管道](../sms/create-sms.md)

1. (選擇性) 定義傳遞[排程](#gs-schedule)。如果未定義排程，在按一下「**[!UICONTROL 傳送]**」按鈕後，訊息會立即傳送。
1. 按一下「**[!UICONTROL 檢閱並傳送]**」按鈕，以檢查您的設定。
1. 使用「**[!UICONTROL 模擬內容]**」按鈕，以測試您的傳遞和個性化設定。若要了解訊息模擬的詳細資訊，請參閱[本章節](../preview-test/preview-test.md)。
1. 按一下「**[!UICONTROL 準備]**」按鈕，以計算目標群體並產生訊息。準備步驟可能需要幾分鐘的時間才能完成。準備完成後，訊息即可用於傳送。萬一出現錯誤，請瀏覽到「**記錄檔**」，檢查警示和警告。
1. 檢查結果，然後按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;按鈕以開始傳送訊息。
1. 傳送訊息後，請瀏覽到「**報告**」章節，以存取關鍵量度。若要了解傳遞報告的詳細資訊，請參閱[本章節](../reporting/delivery-reports.md)。

>[!TAB 建立工作流程中的傳遞]

若要在工作流程中建立傳遞，請依照以下步驟進行：

1. 建立一個工作流程或開啟一個現有的工作流程。[進一步瞭解工作流程](../workflows/gs-workflow-creation.md#gs-workflow-steps)
1. 新增並設定[**[!UICONTROL 建置對象]**](../workflows/activities/build-audience.md)活動。
1. 按一下 `+` 圖示並選取傳遞活動：**[!UICONTROL 電子郵件]**、**[!UICONTROL 簡訊]**、**[!UICONTROL 推播通知 (Android)]** 或&#x200B;**[!UICONTROL 推播通知 (iOS)]**。在[本節](../workflows/activities/channels.md)中進一步瞭解工作流程中的傳遞通道活動，以及如何定義傳遞內容。

   ![](assets/add-delivery-in-wf.png){zoomable="yes"}

1. 啟動工作流程，並檢查記錄檔。

您還可以在不建立工作流程的情況下在行銷活動中新增傳遞。若要這麼做，請瀏覽到行銷活動的「**[!UICONTROL 傳遞]**」標籤，然後按一下「**[!UICONTROL 建立傳遞]**」按鈕。

![](assets/new-campaign-delivery.png){zoomable="yes"}

設定步驟和獨立傳遞類似。

如需有關如何設定行銷活動以及管理屬於行銷活動的傳遞的詳細資訊，請參閱[本章節](../campaigns/gs-campaigns.md)。

>[!ENDTABS]

## 新增個人化 {#personalization}

Adobe Campaign 傳送的資訊可以透過多種方式實現個人化。[深入了解個人化功能](../personalization/gs-personalization.md)。

使用 Campaign 建立動態內容並傳送個人化訊息。可合併個人化功能以改善您的訊息並建立自訂的使用者體驗。

您可以透過以下方式個人化訊息內容：

* 插入動態&#x200B;**個人化欄位**

  個人化欄位用於訊息的第一層個人化。您可以從個人化編輯器選取資料庫中的任何欄位。對於傳遞，您可以選取與收件者、訊息或傳遞相關的任何欄位。可將這些個人化屬性插入訊息的主旨行或內文中。[了解更多](../personalization/personalize.md)

* 正在插入預先定義的&#x200B;**運算式片段**

  Campaign隨附一組運算式片段，其中包含您可以插入傳送中的特定轉譯。 例如，您可以新增標誌、問候訊息或訊息鏡像頁面的連結。運算式片段可從個人化編輯器中的專用專案取得。 此外，您也可以建立自己的運算式片段以符合您的需求。 [瞭解如何使用運算式片段](../content/use-expression-fragments.md)

* 建立&#x200B;**條件式內容**

  例如，設定條件式內容以根據收件者的設定檔新增動態個人化。特定條件為真時，即可插入文字區塊及/或影像。[了解更多](../personalization/conditions.md)

* 新增&#x200B;**個人化優惠方案**

  可根據收件者位置、目前的天氣或上次的採購訂單，在您的訊息內容中插入個人化優惠方案。[了解更多](../msg/offers.md)

## 預覽和測試您的傳遞 

定義訊息內容後，即可進行預覽以控制訊息的呈現，並使用測試設定檔檢查個人化設定。[了解更多](../preview-test/preview-test.md)

## 排程傳遞傳送 {#gs-schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="設定聯絡日期和時間"
>abstract="定義傳送傳遞的日期和確切時間。為您的行銷訊息選擇最合適的時間，可以將開啟率提升至最高。"

您可以設定傳送訊息的日期和確切時間。為您的行銷訊息選擇最合適的時間，可以將開啟率提升至最高。

若要排程傳遞傳送，請開啟傳遞並瀏覽至「**[!UICONTROL 排程]**」章節。使用「**[!UICONTROL 啟用排程]**」切換加以啟動，並設定想要的傳送日期和時間。傳送傳遞後，將在您定義的聯絡日期開始實際傳送。

![](assets/schedule.png){zoomable="yes"}

預設會選取「**[!UICONTROL 啟用傳送前確認]**」選項。此選項要求您在排程的日期和時間傳遞之前確認傳送。如果您需要在排程的日期和時間自動傳送傳遞，您可以停用此選項。

了解[本章節](../monitor/prepare-send.md#schedule-the-send)中傳送排程的傳遞步驟。

## 監視和追蹤記錄 {#gs-tracking-logs}

傳送傳遞後進行監視是確保行銷活動效率並和客戶保持聯繫的關鍵步驟。 

您可以在傳送傳遞後進行監視，並了解如何管理傳遞失敗和隔離。

若要了解監視和追蹤功能的詳細資訊，請參閱[本章節](../reporting/gs-reports.md)。