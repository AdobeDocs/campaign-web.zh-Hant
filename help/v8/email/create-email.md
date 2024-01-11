---
audience: end-user
title: 傳送您的第一個電子郵件
description: 了解如何使用 Campaign Web UI 傳送您的第一個電子郵件
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="有限可用性"
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 67%

---


# 傳送您的第一個電子郵件 {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="開始使用電子郵件"
>abstract="您可以建立獨立的電子郵件傳遞，或在行銷活動工作流程的環境中建立電子郵件。了解如何建立傳遞、選取對象以及設計電子郵件內容。"

了解如何建立您的第一個目標電子郵件。在此使用案例，您排程在特定日期傳送電子郵件給銀級和金級忠誠會員。

根據預先定義的 [設計範本](../email/create-email-templates.md)，該電子郵件也會根據客戶設定檔屬性提供個人化內容。

## 建立電子郵件傳遞 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="選擇電子郵件範本"
>abstract="電子郵件範本是一種特定的傳遞設定，其中包含預先定義的設定，例如類型規則、個人化或路由參數。範本在 Campaign 用戶端主控台中定義。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="定義電子郵件屬性"
>abstract="這些屬性是常見的傳遞參數，可幫助您對傳遞進行命名和分類。附加設定是選擇性的。如果您的傳遞是根據 Adobe Campaign v8 主控台中定義的擴充結構描述，則可使用某些特定&#x200B;**自訂選項**&#x200B;欄位。"

您可以建立獨立的電子郵件傳遞，或在行銷活動工作流程的環境中建立電子郵件。以下步驟詳細說明獨立（一次性）電子郵件傳送的程式。 在中進一步瞭解Adobe Campaign的傳遞建立步驟 [此頁面](../msg/gs-deliveries.md).

若要建立新的獨立電子郵件傳送，請遵循下列步驟。

1. 瀏覽至 **[!UICONTROL 傳遞]** 功能表，然後按一下  **[!UICONTROL 建立傳遞]** 按鈕。

   ![](../msg/assets/create-a-delivery.png)

1. 選取 **[!UICONTROL 電子郵件]** 做為頻道，並從清單中選擇電子郵件傳遞範本。

   >[!NOTE]
   >
   >範本是預先設定的傳遞設定，儲存供未來使用。[了解更多](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. 按一下「**[!UICONTROL 建立傳遞]**」按鈕以確認。
1. 輸入傳遞的標籤並根據您的需要設定其他選項：

   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。
   * **[!UICONTROL 資料夾]**：將傳送儲存在特定資料夾。
   * **[!UICONTROL 傳遞代碼]**：使用此欄位可根據您自己的命名慣例來組織傳送。
   * **[!UICONTROL 說明]**：指定傳送的說明。
   * **[!UICONTROL 性質]**：指定電子郵件的性質以進行分類。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >如果您使用特定自訂欄位擴展結構描述，則可以在「**[!UICONTROL 自訂選項]**」區段存取它們。

   ![](assets/email-properties.png)

1. 此外，進階設定（例如型別規則和目標對應）可透過以下方式存取： **[!UICONTROL 設定]** 按鈕的位置。 這些設定已在選取的範本中預先設定，但可視需要為此特定電子郵件進行編輯。 [了解更多](../advanced-settings/delivery-settings.md)

## 定義對象 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="選取傳遞對象"
>abstract="為您的行銷訊息選取最佳對象。您可以選擇現有對象(已在Campaign v8執行個體中或從Adobe Experience Platform中定義)，使用查詢塑模器建立新對象，或上傳包含對象的檔案。 「**從檔案中選取**」選項未啟用控制組，反之亦然。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="選取主要對象"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="設定控制組"

在此使用案例中，您會傳送電子郵件給現有的對象。

有關如何使用對象的其他說明，請參閱[本章節](../audience/about-recipients.md)。

1. 若要選取電子郵件的對象，請按一下「**[!UICONTROL 選取對象]**」按鈕，然後從清單選擇一個現有對象。

   在此範例中，我們希望使用的現有對象其目標定位為銀級和金級忠誠積分層級的客戶。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >清單中可用的對象源自您的Campaign v8執行個體，或若已在您的執行個體上設定目的地/來源整合，則源自Adobe Experience Platform。 此整合可讓您將Experience Platform區段傳送至Adobe Campaign，並將Campaign傳送和追蹤記錄傳送至Adobe Experience Platform。 瞭解如何在中使用Campaign和Adobe Experience Platform [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. 選取對象後，您可以套用其他規則進一步調整目標。

   ![](assets/audience-selected.png)

1. 您也可以設定控制組來分析電子郵件收件者與非目標收件者相比的行為。[了解如何使用控制組](../audience/control-group.md)

## 定義電子郵件內容 {#create-content}

若要開始建立您的電子郵件內容，請遵循下列步驟。 在此使用案例中，您會使用預先定義的電子郵件 [傳遞範本](../msg/delivery-template.md) 以設計您的電子郵件。<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. 在電子郵件傳遞控制面板中，按一下 **[!UICONTROL 編輯內容]** 按鈕。

   ![](assets/email-edit-content.png)

   這會將您帶到專用介面，您可以在其中設定電子郵件內容並存取電子郵件設計工具。 [了解更多](edit-content.md)

   ![](assets/edit-content.png)

1. 輸入電子郵件的主旨行並使用運算式編輯器加以個人化。[了解如何個人化您的內容](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 若要設計電子郵件的內容，按一下「**[!UICONTROL 編輯電子郵件內文]**」按鈕。

   選擇用於建立電子郵件內容的方法。在此範例中，使用 [預先定義的內容範本](create-email-templates.md).

   ![](assets/select-template.png)

1. 選取範本後，它會顯示在 [電子郵件設計工具](create-email-content.md)，您可在此進行任何必要的編輯並新增個人化。

   例如，若要為電子郵件標題新增個人化，請選取元件區塊，然後按一下「**[!UICONTROL 新增個人化]**」。

   ![](assets/add-perso.png)

1. 一旦您對內容感到滿意，請儲存並關閉您的設計。按一下「**[!UICONTROL 儲存]**」回到電子郵件建立畫面。

   ![](assets/save-content.png)

## 排程傳送 {#schedule}

若要排程電子郵件的傳送，請遵循下列步驟。

有關如何排程傳遞傳送的其他指示，請參閱 [本節](../msg/gs-messages.md#gs-schedule).

1. 瀏覽至 **[!UICONTROL 排程]** 區段。

1. 使用 **[!UICONTROL 啟用排程]** 切換即可啟用。

1. 設定所要的傳送日期和時間。

   ![](assets/schedule.png)

傳送傳遞後，將在您定義的聯絡日期開始實際傳送。

## 預覽和測試電子郵件 {#preview-test}

在傳送電子郵件之前，您可以預覽和測試以確保它符合您的期望。

在此使用案例，您預覽電子郵件並將測試版本傳送到特定電子郵件地址，同時模擬一些目標設定檔。

有關如何預覽和測試電子郵件的其他資訊，請參閱[本章節](../preview-test/preview-test.md)。

1. 若要檢閱您的電子郵件，請按一下「**[!UICONTROL 檢閱並傳送]**」。這將顯示您的電子郵件的預覽，以及所有已設定的屬性、對象和排程。您可以按一下修改按鈕來編輯任何其中一個元素。

1. 若要預覽電子郵件並傳送測試版本，請按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/review-email.png)

1. 在左側，選取要用於預覽電子郵件的設定檔。

   右窗格顯示根據所選設定檔的電子郵件預覽。如果您已新增多個設定檔，您可以切換設定檔以預覽對應的電子郵件。

   ![](assets/preview.png)

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. 若要傳送電子郵件的測試版本，請按一下「**[!UICONTROL 測試]**」按鈕，然後選擇您要使用的模式。

   在此範例中，使用 **[!UICONTROL 主要目標的替代]**&#x200B;模式，其會傳送測試版本至特定電子郵件地址，同時模擬電子郵件的一些目標設定檔。

   ![](assets/proof-mode.png)

1. 按一下「**[!UICONTROL 新增地址]**」並指定會接收測試版本的電子郵件地址。

   對於每個電子郵件地址，選取要模擬的設定檔。您也可以讓 Adobe Campaign 從目標中選取隨機設定檔。

   ![](assets/proof-test-profile.png)

1. 按一下「**[!UICONTROL 傳送測試電子郵件]**」並確認傳送。

   測試版本傳送到特定電子郵件地址，其使用開頭為 **[Proof x]** 的所選設定檔。

   ![](assets/proof-sent.png)

   您可以隨時按一下模擬內容畫面中的「**[!UICONTROL 檢視測試電子郵件記錄]**」按鈕，查看傳送狀態和存取已傳送的測試電子郵件。

## 傳送並監控電子郵件 {#prepare-send}

檢閱並測試電子郵件後，您可以啟動準備作業並傳送。

1. 若要開始準備電子郵件，按一下「**[!UICONTROL 準備]**」。[了解如何準備電子郵件](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 準備好傳送電子郵件後，按一下「**[!UICONTROL 傳送]**」按鈕 (或 **[!UICONTROL 依排程傳送]**，如果您已排程傳送)，然後確認傳送。

1. 在傳送程序期間，您可以直接在此畫面即時追蹤其進度並檢視統計資料。

   ![](assets/sending-email.png)

   <!--
    ![](assets/sent-email.png)-->

   您也可以按一下「**[!UICONTROL 記錄]**」按鈕存取傳送作業的詳細資訊。[了解如何監控傳遞記錄](../monitor/delivery-logs.md)

1. 傳送電子郵件後，您可以按一下「**[!UICONTROL 報告]**」按鈕存取專屬報告以進一步分析。

![](assets/reports.png)
