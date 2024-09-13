---
title: Campaign v8 Web 使用者介面先前發行說明
description: 2024 Campaign Web 使用者介面版本
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 387a69abf4b97cd202c1a7e24bcf14c6af442714
workflow-type: ht
source-wordcount: '1869'
ht-degree: 100%

---

# 2024 年發行說明 {#2024-release}

此頁面列出了 **2024 年版本**&#x200B;的所有變更和改進。最新的發行說明可以在[此頁面](release-notes.md)找到。

## 7 月發行說明 {#24-7-release}

**發行日期**：2024 年 7 月 30 至 31 日

以下功能和改良功能將從 7 月版開始提供。

### 內容片段 {#24-7-1}

您現在可以建立及使用內容片段。內容片段是可重複使用的元件，可在一則或多則訊息中參考。修改片段時，使用該片段的所有內容都會隨之更新。此功能可讓您預先建立多個自訂內容區塊，以便行銷使用者在改進的設計流程中使用這些內容區塊來快速組裝訊息內容。

可用的片段類型有兩種：

* **運算式片段**&#x200B;是預先定義的運算式，可從運算式編輯器的專用項目中取得。
* **視覺片段**&#x200B;是預先定義的視覺區塊，可在多個電子郵件傳遞或內容範本中重複使用。[了解更多](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**視覺片段**&#x200B;為限量開放 (LA) 版本。此功能僅限&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶使用，且無法部署在任何其他環境中。

### 捕捉器群組 {#24-7-2}

**捕捉器群組**&#x200B;是一份種子地址的清單。它用於在您的傳遞中包含特定地址，然後定位與定義的目標標準不相符的設定檔。這樣，不在傳遞客群範圍內的收件者就可以像其他目標收件者一樣接收傳遞內容。您可以在傳送校樣時使用種子地址，或用它來保護您的郵寄清單。[了解更多](../audience/trap-group.md)

### 豐富推播通知範本 {#24-7-3}

您現在可以傳送豐富推播通知。豐富推播通知是行動通知的增強形式，其不僅限於簡單文字訊息，而是結合了多媒體元素，例如影像、互動式按鈕或其他豐富媒體內容。透過此版本，您現在可以在 iOS 和 Android 應用程式中使用一組豐富推播通知範本。

[了解更多](../push/rich-push.md)

>[!AVAILABILITY]
>
>此功能需要更新到 Campaign v8.6.3 <!--or v8.7.2-->。如需詳細資訊，請參閱 Campaign v8 用戶端控制台[發行說明](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}。

### 改良功能 {#improvements-24-7}

**資料夾管理**  - 您現在可以管理資料夾的權限和限制。

## 6 月發行說明 {#24-6-release}

**發行日期**：2024 年 6 月 18-19 日

從 6 月版本開始，所有使用者都可以使用以下功能和改善內容。

### 傳遞警報 {#24-6-3}

「傳送警報」功能是警報管理系統，可讓一組使用者自動接收包含其傳送執行資訊的通知。[閱讀更多](../msg/delivery-alerting.md)

### 計劃和專案 {#24-6-4}

現在您可以建立計劃和專案來組織您的活動。透過定義資料夾階層，您可以將行銷活動組織成專案，並將專案組織成計劃。[閱讀更多](../administration/plans-programs.md)

### 功能改進 {#improvements-24-6}

* **擴充活動中的調和**：**擴充**&#x200B;活動現在可用於調和 Campaign 資料庫結構描述中的資料與其他結構描述中的資料，或來自臨時結構描述的資料 (例如使用載入檔案活動上傳的資料)。例如，您可以使用此選項將上傳檔案中指定的設定檔所在國家/地區與 Campaign 資料庫專用表中可用的國家/地區之一進行調和。[閱讀更多](../workflows/activities/enrichment.md)

## 5 月發行說明 {#24-5-release}

**發行日期**：2024 年 5 月 21 日

從 5 月版本開始，所有使用者都可以使用以下功能和改善內容。

### 稽核軌跡  {#24-5-1}

新的&#x200B;**稽核軌跡**&#x200B;功能會針對您在 Adobe Campaign 執行個體執行的所有動作和事件，即時提供按時間順序排列的詳細記錄。它提供了方便的方法來追蹤行銷活動資料的所有變更，解決各種查詢問題，例如：工作流程狀態、最新修改工作流程的個人，或執行個體內使用者執行的活動。[閱讀更多](../reporting/audit-trail.md)

### 自訂欄位 {#24-5-2}

**自訂欄位**&#x200B;是透過 Adobe Campaign 控制台新增到現成結構描述的附加屬性。在 Campaign Web 使用者介面中，這些自訂欄位現在會在各個畫面中顯示，例如設定檔或測試設定檔的詳細資訊。在 Web 使用者介面中，您無法建立自訂欄位，但現在可以更改自訂欄位的顯示方式。[閱讀更多](../administration/custom-fields.md)

### 建立表格之間的連結 {#24-5-3}

現在您可以在&#x200B;**擴充**&#x200B;工作流程活動中建立與另一個表格的連結。使用活動參數中的新&#x200B;**連結定義**&#x200B;區段，在工作表資料和 Adobe Campaign 資料庫之間建立連結。例如，如果您從包含收件人帳戶、國家/地區和電子郵件的文件載入資料，您現在可以建立指向國家/地區表的連結，以更新其設定檔中的此資訊。[閱讀更多](../workflows/activities/enrichment.md#create-links)

### 一般改善 {#improvements-24-5}

* **直接郵件** - 現在您可以利用運算式編輯器來選取要在直接郵件擷取檔案中顯示的屬性。[閱讀更多](../direct-mail/content-direct-mail.md)

* **資料夾管理** - 現在您可以建立與上層資料夾不同類型的子資料夾。[閱讀更多](../get-started/permissions.md#folders)

* **全球化** - 鑒於我們持續努力統一使用者體驗，因此我們統一了 Adobe Experience Cloud 產品和應用程式中使用的術語。這會影響德語術語「Titel」，當與物件名稱相關時，該術語會改為「Label」。這些變更將在 UI 和文件中逐步推出。


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

請注意，此功能為&#x200B;**限量開放** (LA) 版本。


### 限量開放版本中的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hant)」。

* **品牌化** - 作為 Campaign Standard 移轉使用者，您的技術管理員現在可以定義一或多個品牌，以集中管理影響品牌識別的參數。這包括品牌標誌、登陸頁面存取 URL 之網域或訊息追蹤設定。您可以建立這些品牌，並將其連結至訊息或登陸頁面。 此設定在範本中管理。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-hant)

* **Rest API** - 作為 Campaign Standard 移轉使用者，您可使用 Rest API 來建立 Adobe Campaign 整合，並將 Adobe Campaign 與您使用的技術面板結合，以便建立您自己的生態系統。 [閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-hant)

* **動態報告** - 作為 Campaign Standard 移轉使用者，您可存取動態報告，其提供完全可自訂的即時報告，以便測量行銷活動的影響。 其可新增對設定檔資料的存取權，除了功能性電子郵件行銷活動資料 (如開啟和點按) 外，還可依設定檔維度 (例如，性別、城市和年齡) 進行人口統計分析。[閱讀更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=zh-hant)

* **登陸頁面** - 登陸頁面的以下改善僅適用於從 Campaign Standard 轉換的使用者：

   * 現在，您可以在設定服務時參考預設訂閱/取消訂閱登入頁面。設計電子郵件時，如果您定義指向該登陸頁面的連結，則提交登陸頁面表單的使用者會自動訂閱或取消訂閱此服務。[閱讀更多](../audience/manage-services.md#create-service)
   * 登陸頁面設定中的新選項允許匿名訪客存取登陸頁面。如果取消選擇此選項，則只有已識別的使用者才能存取並提交表單。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 登陸頁面設定中的新選項允許在提交登陸頁面時儲存其他內部資料。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 新選項允許將登陸頁面用於多個服務，使登陸頁面動態化。新增連結到電子郵件時，如果您選擇動態登陸頁面，則可以選取任何服務。如果您選取與特定服務相關的登陸頁面，系統會自動使用該服務 (您無法選取其他服務)。[閱讀更多](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陸頁面現在支援條件內容。[閱讀更多](../landing-pages/lp-content.md)

### 一般改善 {#improvements-24-4}

從 4 月版本開始，所有客戶都可取得以下改善。

* **載入檔案**&#x200B;活動已透過多個部分加強，可讓您上傳範例檔案、管理錯誤和拒絕的內容，以及在活動執行後刪除上傳檔案。[閱讀更多](../workflows/activities/load-file.md)


* 你現在可以在工作流程和不同瀏覽器分頁中的其他工作流程之間&#x200B;**複製/貼上活動**。[閱讀更多](../workflows/orchestrate-activities.md#copy-activities-copy)

* 您現在可以管理所有工作流程活動的&#x200B;**執行選項**。這可讓您定義活動的執行模式和行為，以因應錯誤情況。[閱讀更多](../workflows/orchestrate-activities.md#execution-options-execution)

* **分割活動**&#x200B;中的「如果群體是空的，請勿啟用轉換」選項，可讓您選擇當區段結果為空時工作流程是否應轉換到下一個活動。[閱讀更多](../workflows/activities/split.md)

## 3 月發行說明 {#24-3-release}

>[!AVAILABILITY]
>
>此版本適用於從 [Campaign (控制台) v8.6 發行版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-hant)開始的所有使用者。 請參閱 [Campaign v8 (控制台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-hant){target="_blank"}，了解更多有關 Adob&#x200B;&#x200B;e Campaign 客戶端控制台發行版本和升級。

**發行日期**：2024 年 3 月 19-20 日

### 直接郵件管道 {#24-3-dm}

**直接郵件**&#x200B;管道現已可在工作流程中使用，並可作為獨立傳遞來使用。直接郵件是離線管道，可讓您建立、個人化和產生摘取檔案，並將該檔案與您的直接郵件提供者分享，以便他們傳送郵件給您的客戶。

### 新的變更資料來源工作流程活動 {#24-3-change-data-source}

新的&#x200B;**變更資料來源**&#x200B;目標定位活動可讓您變更工作流程工作表格使用的資料來源。 此活動可讓您跨不同的資料庫管理資料，為您提供更多彈性並改善工作效率。

### 分割工作流程活動的改善 {#24-3-split}

現在您可以使用「**分割**」工作流程活動中的「**在相同表格中產生所有子集**」選項，將所有子集歸類至單一的輸出轉換。

### 查詢建模工具 {#24-3-query-modeler}

* 查詢建模工具現在可在電子郵件設計工具中使用。此工具可讓您在建立條件內容時建立條件。
* 建立自訂條件時，預定義值現在適用於日期類型屬性。
* 無法再於圖中的新轉換上新增運算子。這些運算子只能先新增在現有的轉換中，然後才能篩選組件並歸類在一起。
