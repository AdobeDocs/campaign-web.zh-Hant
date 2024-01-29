---
title: 定義特定於著陸頁面的內容
description: 瞭解如何在Campaign網頁中設計登入頁面特定內容
badge: label="有限可用性"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 13%

---

# 定義特定於著陸頁面的內容 {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="使用內容元件"
>abstract="內容元件指可用於建立登陸頁面版面的空白內容預留位置。若要定義讓使用者能夠選取並提交他們的選擇的特定內容，請使用表單元件。"

編輯登入頁面之任何頁面的內容時，皆已預先填入。

主要頁面是使用者按一下登陸頁面連結後（例如從電子郵件或網站）立即顯示給使用者的頁面。 主要頁面已預先填入 [登入頁面特定表單元件](#use-form-component) 讓使用者能夠選取並提交他們的選擇。 您也可以定義 [登入頁面特定樣式](#lp-form-styles).

若要進一步設計登入頁面內容，您可以使用與電子郵件的相同元件。 [了解更多](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## 使用表單元件 {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="設定表單元件欄位"
>abstract="定義您的收件者將如何從您的登陸頁面查看和提交他們的選擇。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="按一下按鈕時會發生什麼事"
>abstract="定義使用者提交登陸頁面表單後會發生什麼事。"

若要定義可讓使用者從您的登入頁面選取並提交其選擇的特定內容，請使用 **[!UICONTROL 表單]** 元件。 請依照下列步驟以執行此操作。

1. 登入頁面特定 **[!UICONTROL 表單]** 元件已顯示在所選範本的畫布中。

   >[!NOTE]
   >
   >此 **[!UICONTROL 表單]** 元件只能在同一個頁面上使用一次。

1. 選取它。 此 **[!UICONTROL 表單內容]** 標籤會顯示在右側的浮動視窗中，供您編輯表單的不同欄位。

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >切換至 **[!UICONTROL 樣式]** 索引標籤來編輯表單元件內容的樣式。 [了解更多](#lp-form-styles)

1. 展開第一個文字欄位。 從 **[!UICONTROL 文字欄位1]** 區段，您可以編輯欄位型別、來自資料庫的欄位、標籤，以及在使用者填寫欄位之前，顯示在欄位內的文字。

   ![](assets/lp-form-text-field.png)

1. 檢查 **[!UICONTROL 將表單欄位設為必填]** 選項（如果需要）。 在此情況下，只有在使用者已填入此欄位時，才能提交登入頁面。

   >[!NOTE]
   >
   >如果未填入必填欄位，當使用者提交頁面時會顯示錯誤訊息。

1. 新增核取方塊。 選取該核取方塊應該更新資料庫中的服務或欄位。

   ![](assets/lp-form-checkbox.png)

   定義此核取方塊是選擇使用者加入還是退出。 從下列兩個選項中選取：

   * **[!UICONTROL 如果選取，則訂閱]**：使用者需要核取方塊才能同意（選擇加入）。
   * **[!UICONTROL 如果勾選，則取消訂閱]**：使用者需要核取方塊以移除其同意（選擇退出）。

1. 您可以視需要刪除和新增任意數目的文字欄位和/或核取方塊。

1. 新增所有需要的核取方塊和/或文字欄位後，請按一下 **[!UICONTROL 行動號召]** 以展開對應的區段。 它可讓您定義 **[!UICONTROL 表單]** 元件。

   ![](assets/lp-call-to-action.png)

1. 定義按一下按鈕後會發生什麼動作：

   * **[!UICONTROL 確認頁面]**：系統會將使用者重新導向至 **[!UICONTROL 確認]** 為目前登陸頁面設定的頁面。

   * **[!UICONTROL 重新導向URL]**：輸入使用者將重新導向的頁面URL。

1. 如果您想在提交表單時進行其他更新，請選取 **[!UICONTROL 其他更新]**，選擇 **[!UICONTROL 選擇加入]** 或 **[!UICONTROL 選擇退出]**，並定義是否要更新訂閱清單、頻道或只是使用的電子郵件地址。

   ![](assets/lp-form-additionnal-updates.png)

1. 儲存您的內容以返回 [登陸頁面屬性](create-lp.md).

## 定義登陸頁面表單樣式 {#lp-form-styles}

1. 若要修改表單元件內容的樣式，請隨時切換為 **[!UICONTROL 樣式]** 標籤。

   ![](assets/lp_designer-form-style.png)

1. 此 **[!UICONTROL 欄位]** 「區段」預設為展開，可讓您編輯文字欄位的外觀，例如標籤與預留位置字型、標籤位置、欄位背景顏色或欄位邊框。

   ![](assets/lp_designer-form-style-fields.png)

1. 展開 **[!UICONTROL 核取方塊]** 區段來定義核取方塊及對應文字的外觀。 例如，您可以調整字型系列或大小，或是核取方塊框線顏色。

   ![](assets/lp_designer-form-style-checkboxes.png)

1. 展開 **[!UICONTROL 按鈕]** 部分，修改元件表單中按鈕的外觀。 例如，您可以變更字型、新增框線、在游標停留時編輯標籤顏色，或調整按鈕的對齊方式。

   ![](assets/lp_designer-form-style-buttons.png)

   您可以使用來預覽某些設定，例如暫留時的按鈕標籤顏色 **[!UICONTROL 模擬內容]** 按鈕。 進一步瞭解測試登入頁面 [此處](create-lp.md#test-landing-page).

1. 展開 **[!UICONTROL 表單版面配置]** 區段來編輯版面設定，例如背景顏色、邊框間距或邊界。

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

