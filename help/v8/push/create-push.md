---
audience: end-user
title: 建立推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web建立推播通知傳遞
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 30%

---

# 建立推播通知傳遞 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推播通知範本"
>abstract="選取推播通知範本以開始進行推播傳遞。傳遞範本可讓您在行銷活動和傳遞中輕鬆重複使用自訂內容和設定。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=zh-hant" text="使用傳遞範本"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="推播傳遞屬性"
>abstract="定義您的推送傳遞屬性。輸入推播的標籤，並使用「**其他選項**」設定內部名稱、傳遞資料夾和代碼。您也可以輸入自訂說明。"

您可以建立獨立的推播通知傳送，或在行銷活動工作流程的內容中建立推播通知。 以下步驟詳細說明獨立（一次性）推播傳送的程式。 如果您在行銷活動工作流程的內容中工作，建立步驟將在[本節](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow)中詳細說明。

## 建立推播傳遞 {#create-push-delivery}

若要建立新的獨立推送傳送，請遵循下列步驟：

1. 瀏覽至左側邊欄上的&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 建立傳遞]**&#x200B;按鈕。

1. 在&#x200B;**[!UICONTROL 管道]**&#x200B;區段下，選擇&#x200B;**推播通知**&#x200B;作為管道，並根據選擇的裝置作業系統選取範本：Android或iOS。 [進一步瞭解範本](../msg/delivery-template.md)

1. 按一下「**[!UICONTROL 建立傳遞]**」按鈕以確認。

   ![熒幕擷圖顯示已建立推播傳遞](assets/push_create_1.png){zoomable="yes"}

## 設定傳送設定 {#configure-push-settings}

設定您的傳送設定，如下所述：

1. 輸入傳遞的&#x200B;**[!UICONTROL 標籤]**。 依預設，標籤會以所選範本的標籤設定。 應進行更新。

1. 視需要瀏覽&#x200B;**[!UICONTROL 其他選項]**&#x200B;下拉式清單，以自訂選項。 如果您的傳遞是以延伸結構描述為基礎，則可以使用特定的&#x200B;**自訂選項**&#x200B;欄位。

   +++根據您的要求設定下列設定。
   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。
   * **[!UICONTROL 資料夾]**：將傳遞儲存在特定資料夾中。
   * **[!UICONTROL 傳遞代碼]**：使用您自己的命名慣例整理您的傳遞。
   * **[!UICONTROL 說明]**：提供傳遞的說明。
   * **[!UICONTROL 性質]**：指定傳遞的性質，以進行分類。
+++

## 選取您的推播傳遞對象 {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="定義推播通知對象"
>abstract="若要定義訊息客群，您必須先選取與推播傳遞相關聯的應用程式。根據預設，推播通知會傳送給應用程式的所有訂閱者。您可以點選「**選取對象**」按鈕，並調整特定對象的範圍。如果需要，請新增一個控制組來測量傳遞的影響。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=zh-hant" text="設定控制組"

您必須先選取應用程式，然後調整推播通知對象，如下所述：

1. 從&#x200B;**[!UICONTROL 對象]**&#x200B;區段中，選取您要用於此傳遞的應用程式。 根據預設，推播通知會傳送給應用程式的所有訂閱者。您可以按一下&#x200B;**[!UICONTROL 選取對象]**&#x200B;按鈕，以調整為特定對象。

   ![熒幕擷圖顯示推播傳遞的對象選擇](assets/push_create_2.png){zoomable="yes"}

1. 選取現有對象，或建立自己的對象，以調整推播傳送的目標母體。 對於推播通知，預設的[目標維度](../audience/about-recipients.md#targeting-dimensions)為連結至收件者資料表的&#x200B;**訂閱者應用程式** (nms：appSubscriptionRcp)。

   瞭解如何在[此頁面](../audience/add-audience.md)中選取現有對象。

   瞭解如何在[此頁面](../audience/one-time-audience.md)中建立新的對象。

1. 開啟&#x200B;**[!UICONTROL 啟用控制群組]**&#x200B;選項，設定控制群組以測量傳遞的影響。 訊息不會傳送給該控制組，因此您可以將收到訊息的母體的行為與未收到訊息的連絡人的行為進行比較。 [了解更多](../audience/control-group.md)。

## 定義推播通知內容 {#create-content-push}

若要定義通知的內容，請按一下[編輯內容]。**** [了解更多](content-push.md)。

![熒幕擷圖顯示編輯推送傳遞的內容](assets/push_create_5.png){zoomable="yes"}

從這個熒幕，您也可以[模擬您的內容](../preview-test/preview-test.md)和[設定選件](../msg/offers.md)。

## 排程您的傳遞傳送 {#schedule-push}

在工作流程內容中傳送傳遞時，您必須使用&#x200B;**排程器**&#x200B;活動。 在[此頁面](../workflows/activities/scheduler.md)瞭解更多資訊。 下列步驟僅適用於獨立傳送。

若要將獨立推送傳送排程至特定日期和時間，請遵循下列步驟：

1. 瀏覽至傳遞屬性的&#x200B;**[!UICONTROL 排程]**&#x200B;區段。

1. 使用&#x200B;**[!UICONTROL 啟用排程]**&#x200B;切換以啟動它。

1. 設定所要的傳送日期和時間。

當您啟動傳遞後，訊息會在您為收件者定義的確切日期和時間自動傳送。

![熒幕擷圖顯示推播傳遞的排程選項](assets/push_create_3.png){zoomable="yes"}

在[本節](../msg/gs-deliveries.md#gs-schedule)中進一步瞭解傳遞排程。

## 傳遞進階設定 {#adv-push}

按一下&#x200B;**[!UICONTROL 設定傳遞設定]**&#x200B;以存取與傳遞範本相關的進階選項。 [了解更多](../advanced-settings/delivery-settings.md)。

![顯示推播傳遞進階設定的熒幕擷圖](assets/push_create_4.png){zoomable="yes"}