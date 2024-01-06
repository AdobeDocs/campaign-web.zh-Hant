---
audience: end-user
title: 建立推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web建立推播通知傳遞
badge: label="有限可用性"
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 37%

---

# 建立推播通知傳遞 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推播通知範本"
>abstract="選取推播通知範本以開始進行推播傳遞。傳遞範本可讓您在行銷活動和傳遞中輕鬆重複使用自訂內容和設定。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="使用傳遞範本"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="推播傳遞屬性"
>abstract="定義您的推送傳遞屬性。輸入推播的標籤，並使用「**其他選項**」設定內部名稱、傳遞資料夾和代碼。您也可以輸入自訂說明。"

您可以建立獨立的推播通知傳送，或在行銷活動工作流程的內容中建立推播通知。 以下步驟詳細說明獨立（一次性）推播傳送的程式。 如果您在行銷活動工作流程的內容中工作，建立步驟為中的詳細資訊 [本節](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## 建立推播傳遞 {#create-push-delivery}

若要建立新的獨立推送傳送，請遵循下列步驟：

1. 瀏覽至 **[!UICONTROL 傳遞]** 功能表，然後按一下  **[!UICONTROL 建立傳遞]** 按鈕。

1. 在 **[!UICONTROL 頻道]** 區段，選擇 **推播通知** 做為頻道，並根據選擇的裝置作業系統選取範本：Android或iOS。 [進一步瞭解範本](../msg/delivery-template.md)

1. 按一下「**[!UICONTROL 建立傳遞]**」按鈕以確認。

   ![](assets/push_create_1.png)

## 設定傳送設定 {#configure-push-settings}

設定您的傳送設定，如下所述：

1. 輸入 **[!UICONTROL 標籤]** 用於傳遞。 依預設，標籤會以所選範本的標籤設定。 應進行更新。

1. 瀏覽 **[!UICONTROL 其他選項]** 下拉式清單，以視需要自訂選項。 如果您的傳送是以延伸結構描述為基礎，請指定 **自訂選項** 欄位可供使用。

   +++根據您的要求設定下列設定。
   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。
   * **[!UICONTROL 資料夾]**：將傳遞儲存在特定資料夾中。
   * **[!UICONTROL 傳遞代碼]**：使用您自己的命名慣例整理您的傳遞。
   * **[!UICONTROL 說明]**：提供傳遞的說明。
   * **[!UICONTROL 性質]**：指定電子郵件的性質以進行分類。
+++


## 選取您的推播傳遞對象 {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="定義推播通知對象"
>abstract="若要定義訊息對象，您必須先選取與推播傳遞相關聯的應用程式。根據預設，推播通知會傳送給應用程式的所有訂閱者。您可以點選「**選取對象**」按鈕，並調整特定對象的範圍。如果需要，請新增一個控制組來測量傳遞的影響。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="設定控制組"


您必須先選取應用程式，然後調整推播通知對象，如下所述：

1. 從 **[!UICONTROL 對象]** 區段，選取您要用於此傳遞的應用程式。 根據預設，推播通知會傳送給應用程式的所有訂閱者。您可以按一下 **[!UICONTROL 選取對象]** 按鈕。

   ![](assets/push_create_2.png)

1. 選取現有對象，或建立自己的對象，以調整推播傳送的目標母體。 對於推播通知，預設值為 [目標維度](../audience/about-recipients.md#targeting-dimensions) 是 **訂閱者應用程式** (nms：appSubscriptionRcp)，連結至收件者表格。

   瞭解如何在中選取現有對象 [此頁面](../audience/add-audience.md)

   瞭解如何在中建立新受眾 [此頁面](../audience/one-time-audience.md)

1. 切換至 **[!UICONTROL 啟用控制組]** 用來設定控制組以測量傳送影響的選項。 訊息不會傳送給該控制組，因此您可以將收到訊息的母體的行為與未收到訊息的連絡人的行為進行比較。 [了解更多](../audience/control-group.md)

## 定義推播通知內容 {#create-content-push}

若要定義通知的內容，請按一下 **[!UICONTROL 編輯內容]**. [了解更多](content-push.md)

![](assets/push_create_5.png)

在此畫面中，您也可以 [模擬您的內容](../preview-test/preview-test.md) 和 [設定優惠方案](../msg/offers.md).

## 排程您的傳遞傳送 {#schedule-push}

若要將您的傳遞安排在特定的日期和時間，請開啟「**[!UICONTROL 啟用排程]**」選項。在您啟動傳遞後，訊息將在您為收件者定義的確切日期和時間自動傳送。 進一步瞭解中的傳送排程 [本節](../msg/gs-messages.md#gs-schedule)

![](assets/push_create_3.png)


## 傳遞進階設定 {#adv-push}

按一下 **[!UICONTROL 設定傳遞設定]** 以存取與傳送範本相關的進階選項。 [了解更多](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png)
