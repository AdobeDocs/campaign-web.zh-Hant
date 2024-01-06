---
audience: end-user
title: 建立簡訊傳遞
description: 了解如何使用 Adobe Campaign Web 建立並傳送簡訊
badge: label="有限可用性"
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 46%

---

# 建立簡訊傳遞 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="簡訊傳遞屬性"
>abstract="這些屬性包含常見的傳遞參數，可協助您對傳遞進行命名和分類。如果您的傳遞是根據擴充型結構描述完成的，可使用特定的自訂選項欄位。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="定義簡訊對象"
>abstract="您可以建立新對象，或者點選「**選擇對象**」按鈕選取現有的對象。如果需要，請新增一個控制組來測量傳遞的影響。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="設定控制組"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="簡訊範本選取"
>abstract="選取預先定義的範本，以開始進行簡訊傳遞。傳遞範本可讓您在行銷活動和傳遞中輕鬆重複使用自訂內容和設定。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="使用傳遞範本"


您可以建立獨立的SMS傳送，或在行銷活動工作流程的內容中建立SMS。 以下步驟詳細說明獨立（一次性） SMS傳送的程式。 如果您在行銷活動工作流程的內容中工作，建立步驟為中的詳細資訊 [本節](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


若要建立新的獨立SMS傳送，請遵循下列步驟：

1. 瀏覽至 **[!UICONTROL 傳遞]** 功能表，然後按一下  **[!UICONTROL 建立傳遞]** 按鈕。

1. 在 **[!UICONTROL 頻道]** 區段，選擇簡訊作為頻道，並選取範本。 [進一步瞭解範本](../msg/delivery-template.md)

1. 按一下「**[!UICONTROL 建立傳遞]**」按鈕以確認。

   ![](assets/sms_create_1.png)

1. 輸入 **[!UICONTROL 標籤]** 傳送並存取 **[!UICONTROL 其他選項]** 下拉式清單。 如果您的傳送是以延伸結構描述為基礎，請指定 **自訂選項** 欄位可供使用。

   +++根據您的要求設定下列設定。
   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。
   * **[!UICONTROL 資料夾]**：將傳遞儲存在特定資料夾中。
   * **[!UICONTROL 傳遞代碼]**：使用您自己的命名慣例整理您的傳遞。
   * **[!UICONTROL 說明]**：提供傳遞的說明。
   * **[!UICONTROL 性質]**：指定電子郵件的性質以進行分類。
+++

1. 按一下「**[!UICONTROL 選取對象]**」按鈕，以鎖定現有對象或建立您自己的對象。[深入瞭解對象](../audience/about-recipients.md).

   ![](assets/sms_create_2.png)

   瞭解如何在中選取現有對象 [此頁面](../audience/add-audience.md)

   瞭解如何在中建立新受眾 [此頁面](../audience/one-time-audience.md)

1. 切換至 **[!UICONTROL 啟用控制組]** 用來設定控制組以測量傳送影響的選項。 訊息不會傳送給該控制組，因此您可以將收到訊息的母體的行為與未收到訊息的連絡人的行為進行比較。 [了解更多](../audience/control-group.md)

1. 按一下 **[!UICONTROL 編輯內容]** 開始設計簡訊的內容。 [了解更多](content-sms.md)

   ![](assets/sms_create_4.png)

   在此畫面中，您也可以 [模擬您的內容](../preview-test/preview-test.md) 和 [設定優惠方案](../msg/offers.md).

1. 若要將您的傳遞安排在特定的日期和時間，請開啟「**[!UICONTROL 啟用排程]**」選項。在您啟動傳遞後，訊息將在您為收件者定義的確切日期和時間自動傳送。 進一步瞭解中的傳送排程 [本節](../msg/gs-messages.md#gs-schedule).

1. 按一下 **[!UICONTROL 設定]** 以存取與傳送範本相關的進階選項。 [了解更多](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
