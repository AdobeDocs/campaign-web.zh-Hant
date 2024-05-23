---
title: Campaign v8網頁使用者介面發行說明
description: 探索最新Campaign網頁使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 4df01bae0d2099f38012fb082e249bc060e4ce6b
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 81%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 5月發行說明 {#24-5-release}

**發行日期**：2024年5月21日

以下功能和改進專案自5月發行起開放所有使用者使用。

### 稽核軌跡  {#24-5-1}

新的 **稽核軌跡** 功能提供對Adobe Campaign執行個體即時執行的所有動作和事件的詳細時間順序記錄。 它提供一種便利的方法，可追蹤行銷活動資料的所有變更，並解決以下查詢：工作流程的狀態、要修改它們的最新個人，或使用者在執行個體內執行的活動。 [閱讀更多](../reporting/audit-trail.md)

### 自訂欄位 {#24-5-2}

**自訂欄位**&#x200B;是透過 Adobe Campaign 主控台新增到現成結構描述的附加屬性。在 Campaign Web 使用者介面中，這些自訂欄位現在會在各個畫面中顯示，例如設定檔或測試設定檔的詳細資訊。在 Web 使用者介面中，您無法建立自訂欄位，但現在可以更改自訂欄位的顯示方式。[閱讀更多](../administration/custom-fields.md)

### 建立表格之間的連結 {#24-5-3}

您現在可以在以下位置建立與其他表格的連結： **擴充** 工作流程活動。 使用新的 **連結定義** 區段，建立工作表資料與Adobe Campaign資料庫之間的連結。 例如，如果您從包含收件者帳號、國家/地區和電子郵件的檔案載入資料，您現在可以建立指向國家/地區表格的連結，以更新其設定檔中的此資訊。 [閱讀更多](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### 一般改善 {#improvements-24-5}

* **直接郵件**  — 您現在可以運用運算式編輯器來選取要顯示在直接郵件擷取檔案中的屬性。 [閱讀更多](../direct-mail/content-direct-mail.md)

* **資料夾管理**  — 您現在可以建立與父資料夾型別不同的子資料夾。 [閱讀更多](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **全球化**  — 為了提供統一的使用者體驗，我們不斷努力協調Adobe Experience Cloud產品和應用程式中使用的術語。 這會影響德文術語「標題」，在與物件名稱相關時會變更為「標籤」。 這些變更將會逐步在UI和檔案中推出。


## 4 月發行說明 {#april-24-4-release}

**發行日期**：2024 年 5 月 2 日

### 新功能 {#new-24-4}

從 4 月版本開始，所有使用者都可以使用以下功能。

**新的工作流程活動**

* **更新資料** - 使用此活動可以對資料庫中的欄位執行大量更新。您可以透過數個選項，依據個人需求設定資料更新。[閱讀更多](../workflows/activities/update-data.md)
* **訂閱服務**  - 使用此活動可以透過單一動作訂閱或取消訂閱服務的多個設定檔。[閱讀更多](../workflows/activities/subscription-services.md)
* **擷取檔案** - 使用此活動以外部檔案的形式將資料從 Adobe Campaign 匯出到另一個系統。[閱讀更多](../workflows/activities/extract-file.md)
* **傳輸檔案** - 使用此活動可以接收或傳送檔案、測試檔案是否存在或列出伺服器上的檔案。使用的通訊協定可以是伺服器對伺服器通訊協定或 HTTP 通訊協定。[閱讀更多](../workflows/activities/transfer-file.md)
* **測試**  - 使用此活動可以根據指定條件啟用轉換。[閱讀更多](../workflows/activities/test.md)
* **JavaScript 程式碼** - 使用此活動可以在工作流程過程中執行 JavaScript 程式碼片段。[閱讀更多](../workflows/activities/javascript-code.md)
* **外部訊號** - 使用此活動可以從其他工作流程或 API 呼叫觸發工作流程的執行。[閱讀更多](../workflows/activities/external-signal.md)
* **增量查詢** - 使用此活動可以按排程查詢資料庫。每次執行此活動時，都會排除先前執行的結果。這可讓您只鎖定新元素。[閱讀更多](../workflows/activities/incremental-query.md)

**多媒體推播通知範本**

現在您可以透過 Android 發送多媒體推播通知。多媒體推播通知是行動裝置通知的加強版，除了簡單的文字訊息，還可以加入多媒體元素，例如影像、互動式按鈕或其他多媒體內容。[閱讀更多](../push/rich-push.md)

請注意，此功能為&#x200B;**有限可用性** (LA) 版本。


### 有限可用性的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能為有限可用性 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html)」。

* **品牌化** - 作為 Campaign Standard 移轉使用者，您的技術管理員現在可以定義一或多個品牌，以集中管理影響品牌識別的參數。這包括品牌標誌、登陸頁面存取 URL 之網域或訊息追蹤設定。您可以建立這些品牌，並將其連結至訊息或登陸頁面。 此設定在範本中管理。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-Hant)

* **Rest API** - 作為 Campaign Standard 移轉使用者，您可使用 Rest API 來建立 Adobe Campaign 整合，並將 Adobe Campaign 與您使用的技術面板結合，以便建立您自己的生態系統。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-Hant)

* **動態報告** - 作為 Campaign Standard 移轉使用者，您可存取動態報告，其提供完全可自訂的即時報告，以便測量行銷活動的影響。 其可新增對設定檔資料的存取權，除了功能性電子郵件行銷活動資料 (如開啟和點按) 外，還可依設定檔維度 (例如，性別、城市和年齡) 進行人口統計分析。[閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **登陸頁面** - 登陸頁面的以下改善僅適用於從 Campaign Standard 轉換的使用者：

   * 現在，您可以在設定服務時參考預設訂閱/取消訂閱登入頁面。設計電子郵件時，如果您定義指向該登陸頁面的連結，則提交登陸頁面表單的使用者會自動訂閱或取消訂閱此服務。[閱讀更多](../audience/manage-services.md#create-service)
   * 登陸頁面設定中的新選項允許匿名訪客存取登陸頁面。如果取消選擇此選項，則只有已識別的使用者才能存取並提交表單。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 登陸頁面設定中的新選項允許在提交登陸頁面時儲存其他內部資料。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 新選項允許將登陸頁面用於多個服務，使登陸頁面動態化。新增連結到電子郵件時，如果您選擇動態登陸頁面，則可以選取任何服務。如果您選取與特定服務相關的登陸頁面，系統會自動使用該服務 (您無法選取其他服務)。[閱讀更多](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陸頁面現在支援條件內容。[閱讀更多](../landing-pages/lp-content.md)

### 一般改善 {#improvements-24-4}

從 4 月版本開始，所有客戶都可取得以下改善。
<!--**Workflow - Copy/Paste into another tab**: -->

* **載入檔案**&#x200B;活動已透過多個部分加強，可讓您上傳範例檔案、管理錯誤和拒絕的內容，以及在活動執行後刪除上傳檔案。[閱讀更多](../workflows/activities/load-file.md)


* 你現在可以在工作流程和不同瀏覽器分頁中的其他工作流程之間&#x200B;**複製/貼上活動**。[閱讀更多](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 您現在可以管理所有工作流程活動的&#x200B;**執行選項**。這可讓您定義活動的執行模式和行為，以因應錯誤情況。[閱讀更多](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* **分割活動**&#x200B;中的「如果族群是空的，請勿啟用轉換」選項，可讓您選擇當區段結果為空時工作流程是否應轉換到下一個活動。[閱讀更多](../workflows/activities/split.md)



## 3 月發行說明 {#24-3-release}

>[!AVAILABILITY]
>
>此版本適用於從 [Campaign (控制台) v8.6 發行版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hant)開始的所有使用者。 請參閱 [Campaign v8 (控制台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hant){target="_blank"}，了解更多有關 Adob&#x200B;&#x200B;e Campaign 客戶端控制台發行版本和升級。

**發行日期**：2024 年 3 月 19-20 日

### 直接郵件頻道 {#24-3-dm}

**直接郵件**&#x200B;頻道現已可在工作流程中使用，並可作為獨立傳遞來使用。直接郵件是離線頻道，可讓您建立、個人化和產生摘取檔案，並將該檔案與您的直接郵件提供者分享，以便他們傳送郵件給您的客戶。

### 新的變更資料來源工作流程活動 {#24-3-change-data-source}

新的&#x200B;**變更資料來源**&#x200B;目標定位活動可讓您變更工作流程工作表格使用的資料來源。 此活動可讓您跨不同的資料庫管理資料，為您提供更多彈性並改善工作效率。

### 分割工作流程活動的改善 {#24-3-split}

現在您可以使用「**分割**」工作流程活動中的「**在相同表格中產生所有子集**」選項，將所有子集歸類至單一的輸出轉換。

### 查詢建模工具 {#24-3-query-modeler}

* 查詢建模工具現在可在電子郵件設計工具中使用。此工具可讓您在建立條件內容時建立條件。
* 建立自訂條件時，預定義值現在適用於日期類型屬性。
* 無法再於圖中的新轉換上新增運算子。這些運算子只能先新增在現有的轉換中，然後才能篩選組件並歸類在一起。
