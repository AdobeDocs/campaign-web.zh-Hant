---
audience: end-user
title: 傳送您的第一封電子郵件
description: 了解如何使用Campaign網頁UI傳送您的第一封電子郵件
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 773d15912aba9804cbd1ad681f7c02a7433ffa66
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# 傳送您的第一封電子郵件 {#first-email}

![](../assets/do-not-localize/badge.png)

了解如何建立第一個目標式電子郵件。 在此使用案例中，您會排程在特定日期傳送電子郵件給銀級和金級忠誠會員。

電子郵件還根據預先定義的設計範本，提供根據客戶設定檔屬性的個人化內容。

![](assets/delivery-list.png)

## 建立電子郵件 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="選取電子郵件範本"
>abstract="電子郵件範本是特定的傳送設定，包含預先定義的設定，例如類型規則、個人化或路由參數。 範本是在Campaign用戶端主控台中定義。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="電子郵件屬性"
>abstract="屬性是常見的傳送參數，可協助您為傳送命名並分類。 如果您的傳送是以Adobe Campaign v8主控台中定義的延伸架構為基礎，則某些特定 **自訂選項** 欄位。"

1. 若要建立新傳送，請瀏覽至 **[!UICONTROL 傳遞]** ，然後按一下  **[!UICONTROL 建立傳送]** 按鈕。

1. 選擇 **[!UICONTROL 電子郵件]** 作為通道並選擇範本。

   >[!NOTE]
   >
   >範本是預先設定的傳送設定，可儲存以供日後使用。 管理員使用者可在Adobe Campaign Console中建立。 [了解如何使用傳遞範本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. 按一下 **[!UICONTROL 建立傳送]** 按鈕進行確認。
1. 輸入傳送的標籤，並根據您的需求設定其他選項：

   * **[!UICONTROL 內部名稱]**:為傳送指派唯一識別碼，
   * **[!UICONTROL 資料夾]**:將傳遞儲存在特定資料夾中，
   * **[!UICONTROL 傳送代碼]**:使用此欄位，根據您自己的命名慣例來組織傳送，
   * **[!UICONTROL 說明]**:指定傳送的說明，
   * **[!UICONTROL 自然]**:為分類目的指定電子郵件的性質。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >如果您已使用特定自訂欄位擴充架構，則可在 **[!UICONTROL 自訂選項]** 區段。

   ![](assets/email-properties.png)

   此外，進階設定（例如類型規則和目標對應）可按一下傳送名稱旁的按鈕來存取。 這些設定會在選取的範本中預先設定，但可視需要編輯此特定電子郵件。

## 建立電子郵件內容 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="了解如何設計您的電子郵件內容"
>abstract="了解如何使用電子郵件設計工具。"

有關如何配置電子郵件內容的詳細說明，請參閱 [本節](../content/edit-content.md).

在此使用案例中，您會使用預先定義的範本來設計電子郵件。

1. 若要開始建立電子郵件內容，請開啟您的電子郵件傳送，然後按一下 **[!UICONTROL 編輯內容]** 按鈕。

   這可讓您進入專用的介面，您可在其中設定電子郵件內容，並使用電子郵件設計工具進行設計。

   ![](assets/edit-content.png)

1. 輸入電子郵件的主旨行，並使用運算式編輯器加以個人化。 [了解如何個人化您的內容](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 若要設計電子郵件內容，請按一下 **[!UICONTROL 編輯電子郵件內文]** 按鈕。

   選擇用來建立電子郵件內容的方法。 在此範例中，使用預先定義的設計範本。

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. 選取範本後，範本會顯示在電子郵件設計工具中，您可以在其中進行任何必要的編輯和新增個人化。

   例如，若要將個人化新增至電子郵件標題，請選取元件區塊並按一下 **[!UICONTROL 新增個人化]**.

   ![](assets/add-perso.png)

1. 對內容感到滿意後，請儲存並關閉您的設計。 按一下 **[!UICONTROL 儲存]** 返回電子郵件建立畫面。

   ![](assets/save-content.png)

## 定義對象 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="定義對象"
>abstract="選取行銷訊息的最佳對象。 您可以選擇已在Campaign v8例項中定義的現有對象，或從Adobe Experience Platform中選擇，或者您可以使用規則產生器建立新對象。"

在此使用案例中，您會傳送電子郵件給現有對象。 有關如何使用對象的其他指示，請參閱 [本節](../audience/about-audiences.md).

1. 若要選取電子郵件的對象，請按一下 **[!UICONTROL 選取對象]** 按鈕，然後從清單中選擇現有對象。

   在此範例中，我們想使用現有的對象來鎖定屬於銀級和金級忠誠度點數等級的客戶。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >清單中可用的對象來自您的Campaign v8執行個體，或來自Adobe Experience Platform（如果已在執行個體上設定目的地/來源整合）。
   >
   >目的地/來源整合可讓您將Experience Platform區段傳送至Adobe Campaign，以及將促銷活動傳送和追蹤記錄檔傳送至Adobe Experience Platform。 [了解如何搭配Campaign和Adobe Experience Platform使用](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. 選取對象後，您可以套用其他規則以進一步縮小目標。

   您也可以設定控制組，以分析與未鎖定目標者相比之下電子郵件收件者的行為。 [了解如何使用控制組](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 排程傳送 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="排程傳送"
>abstract="定義傳送的日期和確切時間。 選擇最適合您的行銷訊息的時間，即可將開放率最大化。"

若要排程電子郵件的傳送，請開啟您的電子郵件傳送，並瀏覽至 **排程** 區段。 使用 **[!UICONTROL 啟用排程]** 切換以啟動，並設定要傳送的日期和時間。 傳送後，實際傳送將從您定義的聯絡日期開始。

依預設， **[!UICONTROL 在傳送前啟用確認]** 選項。 此選項要求您在排程日期和時間傳送電子郵件之前確認傳送。 如果您需要在排程的日期和時間自動傳送電子郵件，您可以停用此選項。

![](assets/schedule.png)

## 預覽並測試電子郵件 {#preview-test}

在傳送電子郵件之前，您可以先預覽並測試它，以確保它符合您的期望。

在此使用案例中，您會在模擬部分目標設定檔時預覽電子郵件，並將測試版本傳送至特定電子郵件地址。

有關如何預覽和測試電子郵件的其他資訊，請參閱 [本節](../preview-test/preview-test.md).

1. 若要檢閱您的電子郵件，請按一下 **[!UICONTROL 檢閱並傳送]**. 這會顯示您電子郵件的預覽，以及所有已設定的屬性、對象和排程。 您可以按一下修改按鈕來編輯這些元素中的任何一個。

1. 若要預覽電子郵件並傳送測試版本，請按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/review-email.png)

1. 在左側，選取您要用來預覽電子郵件的設定檔。

   右窗格會根據選取的設定檔顯示電子郵件的預覽。 如果您已新增多個設定檔，則可以在它們之間切換，以預覽對應的電子郵件。

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. 若要傳送電子郵件的測試版本，請按一下 **[!UICONTROL 測試]** 按鈕，然後選擇要使用的模式。

   在此範例中，使用 **[!UICONTROL 從主要目標替代]** 模式，模擬電子郵件鎖定的部分設定檔時，會將測試版本傳送至特定電子郵件地址。

   ![](assets/proof-mode.png)

1. 按一下 **[!UICONTROL 添加地址]** 並指定接收測試版本的電子郵件地址。

   針對每個電子郵件地址，選取要模擬的設定檔。 您也可以讓Adobe Campaign從目標中選取隨機設定檔。

   ![](assets/proof-test-profile.png)

1. 按一下 **[!UICONTROL 傳送測試電子郵件]** 並確認傳送。

   測試版本會使用選取的設定檔與 **[校樣x]** 前置詞。

   ![](assets/proof-sent.png)

   您可以按一下 **[!UICONTROL 檢視測試電子郵件記錄]** 按鈕。

## 傳送及監視電子郵件 {#prepare-send}

檢閱並測試您的電子郵件後，您可以啟動其準備工作並傳送。

1. 若要啟動電子郵件準備，請按一下 **[!UICONTROL 準備]**. [了解如何準備電子郵件](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 在您的電子郵件準備就緒後，按一下 **[!UICONTROL 傳送]** 按鈕(或 **[!UICONTROL 依排程傳送]** 如果您已排程傳送)，並確認傳送。

1. 在傳送過程中，您可以直接在此畫面中追蹤進度並即時檢視統計資料。

   ![](assets/sent-mail.png)

   您也可以按一下 **[!UICONTROL 記錄檔]** 按鈕。 [了解如何監視傳送記錄](../monitor/delivery-logs.md)

1. 傳送電子郵件後，您可以按一下 **[!UICONTROL 報表]** 按鈕。

![](assets/reports.png)
