---
title: 定義特定於著陸頁面的內容
description: 瞭解如何在Campaign網頁中設計登入頁面特定內容
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: 4dee53676949282b7c0e7664405b7d5a35ef64d2
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 13%

---

# 定義特定於著陸頁面的內容 {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="使用內容元件"
>abstract="內容元件指可用於建立登陸頁面版面的空白內容預留位置。若要定義讓使用者能夠選取並提交他們的選擇的特定內容，請使用表單元件。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="定義主要頁面設定"
>abstract="使用者點選您的登陸頁面連結 (例如從電子郵件或網站) 後，主要頁面會隨即向使用者顯示。"

您可以編輯登入頁面之任何頁面的內容。

第一個頁面（在使用者按一下登入頁面的連結後立即顯示給使用者）已預先填入 [登入頁面特定表單元件](#use-form-component) 所選範本的<!-- to enable users to select and submit their choices-->.

的內容 **[!UICONTROL 確認]**， **[!UICONTROL 錯誤]** 和 **[!UICONTROL 有效期]** 頁面也會預先填入。 視需要編輯。

您也可以定義 [登陸頁面的樣式](#lp-form-styles).

若要進一步設計登入頁面內容：

* 您可以使用與設計電子郵件時所用的相同元件。 [了解更多](../email/content-components.md#add-content-components)

* 您可以像新增電子郵件一樣將條件式內容新增至登入頁面。 [了解更多](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >此功能在有限可用性(LA)中提供。 僅限於移轉的客戶 **從Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和無法部署在任何其他環境中。

## 使用表單元件 {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="設定表單元件欄位"
>abstract="定義您的收件者將如何從您的登陸頁面查看和提交他們的選擇。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="按一下按鈕時會發生什麼事"
>abstract="定義使用者提交登陸頁面表單後會發生什麼事。"

若要定義可讓使用者從您的登入頁面選取並提交其選擇的特定內容，請編輯 **[!UICONTROL 表單]** 元件。 請依照下列步驟以執行此操作。

1. 登入頁面特定 **[!UICONTROL 表單]** 元件已顯示在所選範本的畫布中。

   >[!NOTE]
   >
   >此 **[!UICONTROL 表單]** 元件只能在同一個頁面上使用一次。

1. 選取它。 此 **[!UICONTROL 表單內容]** 標籤會顯示在右側的浮動視窗中，供您編輯表單的不同欄位。

   ![](assets/lp-form-component.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >切換至 **[!UICONTROL 樣式]** 索引標籤來編輯表單元件內容的樣式。 [了解更多](#lp-form-styles)

1. 展開第一個文字欄位（如果有的話），或使用 **[!UICONTROL 新增]** 按鈕。 從 **[!UICONTROL 文字欄位1]** 區段，您可以編輯欄位型別、要更新的資料庫欄位、標籤，以及在使用者輸入值前顯示在欄位內的文字。

   ![](assets/lp-form-text-field.png){zoomable=&quot;yes&quot;}

1. 檢查 **[!UICONTROL 將表單欄位設為必填]** 選項（如果需要）。 在此情況下，只有在使用者已填入此欄位時，才能提交登入頁面。

   >[!NOTE]
   >
   >如果未填入必填欄位，當使用者提交頁面時會顯示錯誤訊息。

1. 展開核取方塊（如有），或使用 **[!UICONTROL 新增]** 按鈕。 選取該核取方塊應該更新資料庫中的服務或欄位。

   ![](assets/lp-form-checkbox.png){zoomable=&quot;yes&quot;}

   如果您選取 **[!UICONTROL 訂閱與服務]**，選取 [服務](../audience/manage-services.md) 從清單中，並在下列兩個選項之間選擇：

   * **[!UICONTROL 如果選取，則訂閱]**：使用者需要核取方塊才能同意（選擇加入）。
   * **[!UICONTROL 如果勾選，則取消訂閱]**：使用者需要核取方塊以移除其同意（選擇退出）。

   如果您選取 **[!UICONTROL 欄位]**，從屬性清單中選取欄位，然後在下列兩個選項之間選擇：

   * **[!UICONTROL 若勾選則為是]**.<!--TBC-->

   * **[!UICONTROL 若勾選，則否]**.<!--TBC-->

1. 您可以刪除和新增儘可能多的欄位（例如文字欄位、選項按鈕、核取方塊、下拉式清單等） 視需要。

1. 新增或更新所有欄位後，按一下 **[!UICONTROL 行動號召]** 以展開對應的區段。 它可讓您定義 **[!UICONTROL 表單]** 元件。 [了解做法](#define-actions-on-form-submission)

   ![](assets/lp-call-to-action.png){zoomable=&quot;yes&quot;}

1. 儲存您的內容以返回 [登陸頁面屬性](create-lp.md#create-landing-page).

### 定義表單提交的動作 {#define-actions-on-form-submission}

1. 定義按一下按鈕後會發生什麼動作：

   * **[!UICONTROL 確認頁面]**：依預設，系統會將使用者重新導向至 **[!UICONTROL 確認]** 為目前登陸頁面設定的頁面。

   * **[!UICONTROL 重新導向URL]**：輸入使用者將重新導向的頁面URL。

   * **[!UICONTROL 登陸頁面]**：您可以選取另一個登陸頁面，將使用者重新導向至該頁面。 請務必適當地設定選取的登陸頁面。

1. 如果您想在提交表單時進行其他更新，請選取 **[!UICONTROL 其他更新]**，並選取您要更新的專案：
   * 訂閱 [服務](../audience/manage-services.md)  — 在此情況下，定義您要在提交表單時選擇加入或選擇退出使用者。 設計電子郵件時，如果您定義 **[!UICONTROL 登陸頁面]**-type連結至此登入頁面，系統會自動使用選取的服務。 [深入瞭解插入連結](../email/message-tracking.md)

     >[!NOTE]
     >
     >如果您想要搭配此登陸頁面使用數個服務，請使用 **[!UICONTROL 來自URL的服務]** 選項如下所述。

   * 管道 — 填寫表單時使用的電子郵件位址。
   * 所有管道 — 提交表單時，使用者將選擇加入或退出（取決於所選的範本），以結束或離開您品牌在所有管道上的所有通訊。
   * 來自資料庫的欄位 — 從屬性清單中選取欄位，並定義在提交表單時該欄位應設為True或False。

   ![](assets/lp-form-additionnal-updates.png){zoomable=&quot;yes&quot;}

1. 選取 **[!UICONTROL 來自URL的服務]** 允許登入頁面用於數個服務的選項，使其成為動態的。 定義您要在提交表單時選擇加入或選擇退出使用者。

   >[!AVAILABILITY]
   >
   >此功能在有限可用性(LA)中提供。 僅限於移轉的客戶 **從Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和無法部署在任何其他環境中。

   ![](assets/lp-form-service-from-url.png){zoomable=&quot;yes&quot;}

   設計電子郵件時，如果您定義 **[!UICONTROL 登陸頁面]**-type連結至此登入頁面，您就可以從清單中選取任何服務。 接著，您可以在定義此登入頁面的其他連結時，選取其他服務。 [深入瞭解插入連結](../email/message-tracking.md)

   ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

## 定義登陸頁面表單樣式 {#lp-form-styles}

1. 若要修改表單元件內容的樣式，請隨時切換為 **[!UICONTROL 樣式]** 標籤。

1. 此 **[!UICONTROL 文字欄位]** 區段預設為展開。 它可讓您編輯文字欄位的外觀，例如標簽字型、標籤位置、欄位背景顏色或欄位邊框。

   ![](assets/lp-text-styles.png){zoomable=&quot;yes&quot;}

1. 展開 **[!UICONTROL 核取方塊]** 區段來定義核取方塊及對應文字的外觀。 例如，您可以調整字型系列和大小，或是核取方塊框線顏色。

   ![](assets/lp-checkbox-style.png){zoomable=&quot;yes&quot;}

1. 展開並編輯與您可能新增的其他欄位（選項按鈕、下拉式清單、日期和時間等）對應的任何其他區段 至您的表單。

1. 展開 **[!UICONTROL 行動號召]** 部分，修改元件表單中按鈕的外觀。 例如，您可以變更字型、新增框線、在游標停留時編輯標籤顏色，或調整按鈕的對齊方式。

   ![](assets/lp-call-to-action-style.png){zoomable=&quot;yes&quot;}

   您可以使用來預覽某些設定，例如暫留時的按鈕標籤顏色 **[!UICONTROL 模擬內容]** 按鈕。 [了解更多](create-lp.md#test-landing-page)

1. 儲存您的變更。
