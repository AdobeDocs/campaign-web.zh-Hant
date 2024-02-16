---
title: 設定登陸頁面
description: 瞭解如何在Campaign網頁中設定和發佈登入頁面
feature: Landing Pages
source-git-commit: 26c41105a4c04b72e0aedf05a4b3268b0e475d40
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 24%

---

# 建立和發佈登陸頁面 {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="建立和管理登陸頁面"
>abstract="Adobe Campaign 可讓您建立、設計和分享登陸頁面，將使用者導向線上網頁；您可以在這些網頁中根據內建範本來管理贏取、訂閱/取消訂閱和封鎖清單使用案例。"

Campaign Web使用者介面可讓您建立、設計和發佈登入頁面。 發佈後，您可以在傳送中插入表單連結。 收件者按一下該連結後，即會被導向相對應的登陸頁面。

[!DNL Adobe Campaign] 隨附四個範本，用於管理下列使用案例： **贏取**， **訂閱**， **取消訂閱**、和 **封鎖清單**.

## 存取登陸頁面 {#access-landing-pages}

若要存取登入頁面清單，請選取 **[!UICONTROL 行銷活動管理]** > **[!UICONTROL 登陸頁面]** 從左側功能表。

![](assets/lp-inventory.png){zoomable=&quot;yes&quot;}

此 **[!UICONTROL 登陸頁面]** 「庫存管理系統」會顯示所有已建立的料號。 您可以使用 **顯示篩選器** 按鈕。 您可以將結果限製為特定 [資料夾](../get-started/permissions.md#folders) 使用下拉式清單，或使用以下專案新增規則： [查詢模型工具](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png){zoomable=&quot;yes&quot;}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>您無法在Campaign網頁使用者介面中顯示或編輯從使用者端主控台（網頁表單）建立的登入頁面。 進一步瞭解 [Campaign主控台檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

您可以複製或刪除登入頁面。 按一下登入頁面旁的省略符號，以選取所需的動作。

## 設定登陸頁面 {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="定義登錄頁面屬性"
>abstract="填寫屬性欄位 (例如標籤) 並根據需要修改綱要。此外，您還可以編輯內部名稱、變更儲存登陸頁面的資料夾和提供說明。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="定義每個頁面的內容"
>abstract="調整屬於此登陸頁面的每個頁面內容，例如表單本身、提交表單時顯示的確認頁面或發生錯誤時引導使用者的頁面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="排程登陸頁面"
>abstract="您可以定義登陸頁面的開始日期和結束日期。當頁面有效期限結束時，就無法再使用該表格。會改為顯示&#x200B;**有效期**&#x200B;頁面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="定義主要頁面設定"
>abstract="使用者點選您的登陸頁面連結 (例如從電子郵件或網站) 後，主要頁面會隨即向使用者顯示。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="設定訂閱登陸頁面"
>abstract="訂閱頁面可讓您的客戶訂閱服務。"

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

若要建立登入頁面，請執行下列步驟：

1. 從 **[!UICONTROL 登陸頁面]** 詳細目錄，按一下 **[!UICONTROL 建立登陸頁面]**.

   ![](assets/lp-create-button.png){zoomable=&quot;yes&quot;}

1. 選取範本：
   * **[!UICONTROL 贏取]**：這是登入頁面的預設範本，可讓您擷取和更新設定檔資料。
   * **[!UICONTROL 訂閱]**：使用此範本讓使用者訂閱特定的 [服務](../audience/manage-services.md).
   * **[!UICONTROL 取消訂閱]**：此範本可用於傳送給服務訂閱者的傳遞，讓他們從此取消訂閱 [服務](../audience/manage-services.md).
   * **[!UICONTROL 封鎖清單]**：當設定檔點按傳送中的選擇退出連結時，且不想再聯絡時，應使用此範本。

   ![](assets/lp-templates.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >瞭解如何在中實施每個範本的不同使用案例 [此頁面](lp-use-cases.md).

1. 按一下 **[!UICONTROL 建立]**.

1. 填入 **[!UICONTROL 屬性]** 欄位，例如標籤。

   根據預設，登入頁面會儲存在 **[!UICONTROL 網頁應用程式]** 資料夾。 您可以瀏覽至中所需的位置來變更它 **[!UICONTROL 其他選項]**. [瞭解如何使用資料夾](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png){zoomable=&quot;yes&quot;}

1. 在 **[!UICONTROL 資料預先載入]** 部分，預設會選取以下兩個選項：

   * 當 **[!UICONTROL 使用表單中參照的資料預先填寫]** 選項經已選取，若登入頁面的訪客符合資料庫中的設定檔，則會自動在表單中預先載入設定檔的資訊。 使用者只需填寫缺少的欄位，並在需要時更新現有值。 這可合併現有設定檔的資料，而非建立重複專案。

   * 此 **[!UICONTROL 如果沒有ID，則跳過預先載入]** 如果您不想更新設定檔，則必須選取選項。 在這種情況下，在核准表單後，輸入的每個設定檔都將新增到資料庫。 例如，在網站上張貼表單時，會使用此選項。

1. 登入頁面可以有後續頁面。 若要新增頁面，請瀏覽 **[!UICONTROL 頁面]** 區段，然後按一下 **[!UICONTROL 編輯內容]** 按鈕來指定您要為此登入頁面設計的每個頁面。 每個頁面的內容均已預先填滿。 視需要編輯。 [了解更多](lp-content.md)

   ![](assets/lp-pages.png){zoomable=&quot;yes&quot;}

1. 此 **[!UICONTROL 更新預先載入的記錄]** 選項預設為選取。 它可讓您透過登入頁面更新儲存在資料庫中的設定檔。 預先載入方塊可讓您指定如何在資料庫中尋找要更新的記錄。

   您也可以從登入頁面目前前後關聯中的欄位中進行選擇，這些欄位將用於尋找資料庫中的對應設定檔。 若要這麼做，請取消選取 **[!UICONTROL 更新預先載入的記錄]** 選項並核取底下的所需欄位 **[!UICONTROL 調解選項]**.

   ![](assets/lp-storage.png){zoomable=&quot;yes&quot;}

1. 您可以定義登陸頁面的開始日期和結束日期。選取 **[!UICONTROL 啟用排程]** 並設定日期。

   ![](assets/lp-schedule.png){zoomable=&quot;yes&quot;}

   * 登入頁面會在指定的開始日期/時間自動發佈。

     >[!NOTE]
     >
     >如果未定義開始日期，登入頁面在發佈後就會立即上線。

   * 當頁面到達結束日期時， <!--the landing page is automatically unpublished and -->表單已無法使用。 會改為顯示&#x200B;**[!UICONTROL 有效期]**&#x200B;頁面。

     >[!NOTE]
     >
     >基於安全性原因和平台效能，Adobe建議您設定結束日期。

1. 按一下 **[!UICONTROL 檢閱和發佈]**.

在您定義所有設定和 [設計](lp-content.md) 您可以 [測試](#test-landing-page) 和 [發佈](#publish-landing-page) 您的登陸頁面，如下所述。

## 測試登陸頁面 {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="模擬登陸頁面"
>abstract="您可以在 Campaign Web 使用者介面中查看登陸頁面的預覽內容，或在新的 Web 瀏覽器標籤中開啟它。"

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="預覽和測試您的登陸頁面"
>abstract="定義登陸頁面設定和內容後，您就可以使用測試設定檔進行預覽。"

定義登入頁面設定和內容後，您就可以使用測試設定檔來預覽。 如果您已插入 [個人化內容](../personalization/gs-personalization.md)，您將能使用測試設定檔資料檢查此內容在登入頁面中的顯示方式。

>[!CAUTION]
>
>您必須有可用的測試設定檔，才能預覽訊息和傳送校樣。 [進一步瞭解測試設定檔](../audience/test-profiles.md)

若要測試您的登入頁面，請遵循下列步驟：

1. 在您按一下 **[!UICONTROL 檢閱和發佈]**，選取 **[!UICONTROL 模擬內容]** 按鈕，存取測試設定檔選取專案。

   ![](assets/lp-simulate-content.png){zoomable=&quot;yes&quot;}

1. 從 **[!UICONTROL 模擬]** 畫面，選取一或多個測試設定檔。

   選取測試設定檔的步驟與測試訊息時相同。 在中會詳細說明這些步驟 [預覽和測試](../preview-test/preview-test.md) 區段。

1. 選取 **[!UICONTROL 開啟預覽]** 以測試您的登入頁面。

   ![](assets/lp-open-preview.png){zoomable=&quot;yes&quot;}

1. 登入頁面的預覽會在新標籤中開啟。 個人化元素會由選取的測試設定檔資料取代。

   如果您已選取 **[!UICONTROL 使用表單中參照的資料預先填寫]** 選項時，表單欄位會自動預先填入對應的測試設定檔資料。<!--TBC-->

   ![](assets/lp-preview.png){zoomable=&quot;yes&quot;}

1. 選取其他測試設定檔以預覽登陸頁面每個變體的呈現。

<!--Can you preview Confirmation/Error/Expiration pages?-->

## 發佈登陸頁面 {#publish-landing-page}

在您的登入頁面準備就緒並完成驗證後，請發佈該頁面，以便使用對應按鈕將其用於傳送中。

發佈後：

* 登入頁面會新增至登入頁面清單，並包含 **[!UICONTROL 已發佈]** 狀態。 它現在已上線，並準備好在您的內容中參照。

* 您可以複製並貼上 **[!UICONTROL 登陸頁面URL]** 會顯示在頁面頂端，並透過網頁瀏覽器預覽您的登陸頁面。

>[!CAUTION]
>
>若要全面測試或善用您的登陸頁面，您不得將此連結直接複製並貼上到網頁瀏覽器或您的傳遞內容中。請改用 [模擬內容](#test-landing-page) 函式進行測試，並遵循中所述的步驟 [本節](lp-use-cases.md) 以正確使用您的登入頁面。

![](assets/lp-published.png){zoomable=&quot;yes&quot;}

您可以透過記錄檔監控登入頁面影響<!--and specific reports-->. 按一下 **[!UICONTROL 記錄檔]** 按鈕。
