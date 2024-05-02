---
title: 最新發行說明
description: 探索 Campaign Web 使用者介面隨附的新增功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ba187eaebf299e5d2ee303c4e15180d35a9e6180
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 25%

---

# 發行說明 {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，通過該模型可採用更具擴充性、分階段的方式部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 4月發行說明 {#april-24-4-release}

**發行日期**：2024年4月30日

### 新功能 {#new-24-4}

以下功能自4月發行版本開始可供所有使用者使用。

**新工作流程活動**

* **更新資料**  — 使用此活動對資料庫中的欄位執行大量更新。 數個選項可讓您個人化資料更新。 [閱讀更多](../workflows/activities/update-data.md)
* **訂閱服務**  — 使用此活動在單一動作中訂閱或取消訂閱多個設定檔至/來自服務。 [閱讀更多](../workflows/activities/subscription-services.md)
* **擷取檔案**  — 使用此活動可將資料從Adobe Campaign匯出至另一個系統，作為外部檔案。 [閱讀更多](../workflows/activities/extract-file.md)
* **傳輸檔案**  — 使用此活動來接收或傳送檔案、測試檔案是否存在或列出伺服器上的檔案。 使用的通訊協定可以是伺服器對伺服器通訊協定或HTTP通訊協定。 [閱讀更多](../workflows/activities/transfer-file.md)
* **測試**  — 使用此活動可根據指定的條件啟用轉換。 [閱讀更多](../workflows/activities/test.md)
* **javascript程式碼**  — 使用此活動在工作流程內容中執行JavaScript程式碼片段。 [閱讀更多](../workflows/activities/javascript-code.md)
* **外部訊號**  — 使用此活動從另一個工作流程*或API呼叫觸發工作流程執行。 [閱讀更多](../workflows/activities/external-signal.md)
* **增量查詢**  — 使用此活動可依排程查詢資料庫。 每次執行此活動時，都會排除先前執行的結果。這可讓您僅鎖定新元素。 [閱讀更多](../workflows/activities/incremental-query.md)

**豐富推送通知範本**

您現在可以透過Android傳送豐富推送通知。 豐富推播通知是行動通知的增強型形式，其不僅限於簡單的文字訊息，而是結合多媒體元素，例如影像、互動按鈕或其他豐富媒體內容。 [閱讀更多](../push/rich-push.md)

請注意，此功能位於 **可用性限制** (LA)。

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### 有限可用中的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>下列功能屬於「有限可用性(LA)」。 限製為移轉的客戶 **從Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和無法部署在任何其他環境中。
>
>請參閱下列檔案頁面： [Campaign Standard轉換至Campaign v8](../rn/acs-migration.md) 和 [Campaign Standard使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **品牌化**  — 作為Campaign Standard移轉的使用者，您的技術管理員現在可以定義一個或多個品牌，以集中影響品牌識別的引數。 這包括品牌標誌、登錄頁面存取 URL 之網域或訊息追蹤設定。您可以建立這些品牌，並將其連結至訊息或登入頁面。 此設定在範本中管理。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API**  — 身為Campaign Standard移轉使用者，您可以使用Rest API來建立Adobe Campaign的整合，並將Adobe Campaign與您使用的技術面板結合，以建立您自己的生態系統。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **動態報告**  — 作為Campaign Standard移轉的使用者，您可以存取動態報告，其提供完全可自訂的即時報告，以評估行銷活動的影響。 它新增對設定檔資料的存取權，除了功能性電子郵件促銷活動資料（如開啟和點按）外，還支援依設定檔維度（如性別、城市和年齡）進行人口統計分析。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **載入檔案活動改善** - **載入檔案** 活動已增強，包含多個區段，可讓您上傳範例檔案、管理錯誤和拒絕，以及在活動執行後刪除已上傳的檔案。 [閱讀更多](../workflows/activities/load-file.md)

* **登陸頁面**  — 下列登陸頁面改良功能僅適用於從Campaign Standard轉換的使用者：

   * 您現在可在設定服務時，參考預設的訂閱/取消訂閱登陸頁面。 設計電子郵件時，如果您定義該登入頁面的連結，則提交登入頁面表單的使用者會自動訂閱或取消訂閱此服務。 [閱讀更多](../audience/manage-services.md#create-service)
   * 登入頁面設定中的新選項可讓匿名訪客存取登入頁面。 如果您取消選取此選項，則只有已識別的使用者才能存取及提交表單。 [閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 登入頁面設定中的新選項可讓您在提交登入頁面時儲存其他內部資料。 [閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 新選項可讓您將登入頁面用於數個服務，使其成為動態頁面。 將連結新增至電子郵件時，如果您選取動態登入頁面，則可選取任何服務。 如果您選取的登入頁面有相關聯的特定服務，此服務將會自動使用（您無法選取其他服務）。 [閱讀更多](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登入頁面現在支援條件式內容。 [閱讀更多](../landing-pages/lp-content.md)

### 一般改善 {#improvements-24-4}

自4月發行版本開始，所有客戶皆可使用以下改良功能。
<!--**Workflow - Copy/Paste into another tab**: -->

* 您現在可以從不同的瀏覽器標籤將活動從工作流程複製/貼上到另一個工作流程。 [閱讀更多](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 現在，所有工作流程活動都可讓您管理其執行選項。 這可讓您定義活動的執行模式和發生錯誤時的行為。 [閱讀更多](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* 中的「如果母體為空白，則不要啟動轉變」選項 **分割活動** 可讓您選擇當區段結果為空白時，工作流程是否應轉換為下一個活動。 [閱讀更多](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* 自訂欄位是透過Adobe Campaign主控台新增到現成可用方案的其他屬性。 在Campaign網頁使用者介面中，這些自訂欄位現在會顯示在各種畫面中，例如設定檔或測試設定檔的詳細資訊。 在Web使用者介面中，您無法建立自訂欄位，但您現在可以修改其顯示方式。 [閱讀更多](../administration/custom-fields.md)


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

您現在可以使用 **在相同表格中產生所有子集** 中的選項 **Split** 工作流程活動，將所有子集分組為單一輸出轉變。

### 查詢建模工具 {#24-3-query-modeler}

* 查詢建模工具現在可在電子郵件設計工具中使用。它可讓您在建立條件式內容時建置條件。
* 建立自訂條件時，預先定義的值現在可用於日期型別屬性。
* 無法再於圖中的新轉換上新增運算子。它們只能在篩選元件以將它們分組之前，新增到現有轉變上。
