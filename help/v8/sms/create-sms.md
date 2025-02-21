---
audience: end-user
title: 建立簡訊傳遞
description: 了解如何使用 Adobe Campaign Web 建立並傳送簡訊
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 43%

---

# 建立簡訊傳遞 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="簡訊傳遞屬性"
>abstract="這些屬性包含常見的傳遞參數，可協助您對傳遞進行命名和分類。如果您的傳遞是根據擴充型結構描述完成的，可使用特定的自訂選項欄位。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="定義簡訊客群"
>abstract="您可以建立新對象，或者點選「**選擇對象**」按鈕選取現有的對象。如果需要，請新增一個控制組來測量傳遞的影響。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=zh-hant" text="設定控制組"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="簡訊範本選取"
>abstract="選取預先定義的範本，以開始進行簡訊傳遞。傳遞範本可讓您在行銷活動和傳遞中輕鬆重複使用自訂內容和設定。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=zh-hant" text="使用傳遞範本"


您可以建立獨立的SMS傳送，或在行銷活動工作流程的內容中建立SMS。 以下步驟詳細說明獨立（一次性） SMS傳送的程式。 如果您在行銷活動工作流程的內容中工作，建立步驟為[此區段](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow)中的詳細資料。


若要建立新的獨立SMS傳送，請遵循下列步驟：

1. 瀏覽至左側邊欄上的&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 建立傳遞]**&#x200B;按鈕。

1. 在&#x200B;**[!UICONTROL 管道]**&#x200B;區段下，選擇簡訊作為管道，然後選取範本。 [進一步瞭解範本](../msg/delivery-template.md)

1. 按一下「**[!UICONTROL 建立傳遞]**」按鈕以確認。

   ![](assets/sms_create_1.png){zoomable="yes"}

1. 輸入傳遞的&#x200B;**[!UICONTROL 標籤]**，並存取&#x200B;**[!UICONTROL 其他選項]**&#x200B;下拉式清單。 如果您的傳遞是以延伸結構描述為基礎，則可以使用特定的&#x200B;**自訂選項**&#x200B;欄位。

   +++根據您的要求設定下列設定。
   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。
   * **[!UICONTROL 資料夾]**：將傳遞儲存在特定資料夾中。
   * **[!UICONTROL 傳遞代碼]**：使用您自己的命名慣例整理您的傳遞。
   * **[!UICONTROL 說明]**：提供傳遞的說明。
   * **[!UICONTROL 性質]**：指定傳遞的性質，以進行分類。
+++

1. 按一下「**[!UICONTROL 選取客群]**」按鈕，以選擇現有客群或建立您自己的客群。[進一步瞭解對象](../audience/about-recipients.md)。

   ![](assets/sms_create_2.png){zoomable="yes"}

   瞭解如何在[此頁面](../audience/add-audience.md)中選取現有對象

   瞭解如何在[此頁面](../audience/one-time-audience.md)中建立新的對象

1. 開啟&#x200B;**[!UICONTROL 啟用控制群組]**&#x200B;選項，設定控制群組以測量傳遞的影響。 訊息不會傳送給該控制組，因此您可以將收到訊息的母體的行為與未收到訊息的連絡人的行為進行比較。 [了解更多](../audience/control-group.md)

1. 按一下&#x200B;**[!UICONTROL 編輯內容]**，開始設計簡訊的內容。 [了解更多](content-sms.md)

   ![](assets/sms_create_4.png){zoomable="yes"}

   從這個熒幕，您也可以[模擬您的內容](../preview-test/preview-test.md)和[設定選件](../msg/offers.md)。

1. 若要將您的傳遞安排在特定的日期和時間，請開啟「**[!UICONTROL 啟用排程]**」選項。在您啟動傳遞後，訊息將在您為收件者定義的確切日期和時間自動傳送。 在[本節](../msg/gs-deliveries.md#gs-schedule)中進一步瞭解傳遞排程。

   >[!NOTE]
   >
   >在工作流程內容中傳送傳遞時，您必須使用&#x200B;**排程器**&#x200B;活動。 在[本頁](../workflows/activities/scheduler.md)中瞭解更多。

1. 按一下&#x200B;**[!UICONTROL 設定]**&#x200B;以存取與您的傳遞範本相關的進階選項。 [了解更多](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable="yes"}
