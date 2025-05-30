---
title: Campaign v8 Web 使用者介面先前發行說明
description: 2025 Campaign Web 使用者介面版本
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 8ec342d565bc8418c202cdba834d74a99cff3a47
workflow-type: ht
source-wordcount: '1281'
ht-degree: 100%

---

# 2025 年發行說明 {#2025-release}

此頁面列出了 **2025 年版本**&#x200B;的所有變更和改進。最新的發行說明可以在[此頁面](release-notes.md)找到。

## 2025 年 4 月版 {#25-4-release}

**發行日期**：2025 年 4 月 29 日

### 新功能 {#25-4-features}

從 4 月版本開始，所有使用者都可以使用以下功能。

<table>
<thead>
<tr>
<th><strong>呼叫中心管道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>呼叫中心管道現在已可在 Campaign Web 使用者介面中取得。此管道是指用於管理和追蹤透過呼叫中心處理的通訊或互動的通訊方法 — 通常是專員撥打給客戶或潛在客戶的電話。</p>
<p>注意：Web UI 中不提供呼叫中心管道的報告功能。您必須瀏覽到用戶端控制台才能存取報告。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>如需詳細資訊，請參閱<a href="../call-center/gs-call-center.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新的規則產生器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以使用新的規則產生器，協助您在改進的使用者介面中定義複雜的條件。您可以視需要從舊的規則產生器切換到新的規則產生器。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>如需詳細資訊，請參閱<a href="../query/query-modeler-overview.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部帳戶製作</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>身為 Campaign 管理員，您現在可以從 Campaign Web 使用者介面中建立與外部系統的新連線。
您也可以檢視、更新和管理現有的外部帳戶。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改良功能 {#25-4-improvements}

**一般使用者介面改善**

* 現在，使用者介面中可以更清楚地看到結構描述屬性的「欄位說明」、「新增至最愛項目」和「數值分佈」選項。如需詳細資訊，請參閱[詳細說明文件](../get-started/attributes.md)。
* 在介面中，日期和時間現在會根據 Experience League 偏好設定中設定的主要語言來進行顯示。這項改進僅適用於幾種語言。若要查看受支援語言的完整清單，請參閱[詳細說明文件](https://experienceleague.adobe.com/zh-hant/docs/core-services/interface/features/browser-language){target=_blank}。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**電子郵件編輯器**：為了增強 Campaign Web 使用者介面中的可存取性，電子郵件設計工具中現在提供兩個新欄位：它們對應至您電子郵件內容的 `html` 元素中的 `title` 元素和 lang 屬性。除了「預覽文字」欄位之外，您還可以在電子郵件的「內文」區段中定義這些設定。如需詳細資訊，請參閱[詳細說明文件](../email/metadata.md)。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**結構描述**

* 您現在可以從 Campaign Web 使用者介面中編輯清單的臨時結構描述。如需詳細資訊，請參閱[詳細說明文件](../audience/manage-audience.md)。
* 您現在可以在範例畫面中預覽結構描述的自訂欄位。如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。
* 您現在可以使用拖放方式，移動清單中的自訂欄位。如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。


### 限量開放版本中的新功能 {#25-4-features-la}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。這些功能需要將 Campaign 伺服器升級到 v8.7.4。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hant)」。

* **建立多語言傳遞** - 您現在可以在 Adobe Campaign Web 使用者介面中，使用不同語言傳送多個電子郵件傳遞。多語言傳遞功能可讓您選擇傳遞的預設語言，以及可以傳送傳遞的不同語言。您也可以使用您選擇的語言來預覽這些傳遞。如需詳細資訊，請參閱[詳細說明文件](../email/edit-content.md)。

* **多語言動態報告** - 動態報告現可用於多語言電子郵件傳遞。如需詳細資訊，請參閱[詳細說明文件](../reporting/global-reports.md)。

* **簡訊 REST API 支援 (LA)** - 交易型傳訊 REST API 現在已可用於簡訊管道。當承載中同時存在 email 和 mobilePhone 時，您可以使用「wishedChannel」欄位來指定管道。如果未提供，除非 wishedChannel 明確地要求簡訊，否則預設會使用電子郵件。如需詳細資訊，請參閱[詳細說明文件](https://experienceleague.adobe.com/zh-hant/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}。

## 2025 年 2 月版 {#25-2-release}

**發行日期**：2025 年 2 月 18 日

以下功能和改良功能將從 2 月版開始提供。

### 功能 {#25-2-features}

<table>
<thead>
<tr>
<th><strong>建立業務規則 (類型規則)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 使用者介面中建立類型和類型規則。您可以使用類型來控制、篩選及優先處理傳遞內容的傳送。類型可用於驗證傳遞是否始終包含強制元件 (例如取消訂閱連結或主旨列)，或套用篩選規則以從您的客群中排除群組 (例如取消訂閱者、競爭者或非忠誠客戶)。</p>
<img src="assets/do-not-localize/typology.gif">
<p>如需詳細資訊，請參閱<a href="../administration/typologies.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>目標對應</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>現在您可以在 Campaign Web 使用者介面中建立目標對應。目標對應定義了不同的傳遞管道 (電子郵件、簡訊、推播通知) 如何連結到結構描述的資料欄位。目標對應可讓您定義目標客群：輪廓、合約受益人、操作者、訂閱者、潛在客戶等。</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>如需詳細資訊，請參閱<a href="../administration/target-mappings.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>結構描述詳細資料</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>現在您可以在清單中選取結構描述的名稱來存取其詳細資料。自訂欄位版本現在可以透過結構描述詳細資料中的「<b>編輯自訂欄位</b>」按鈕存取。</p>
<img src="assets/do-not-localize/schemas.gif">
<p>如需詳細資訊，請參閱<a href="../administration/schemas.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

## 2025 年 1 月版 {#25-1-release}

**發行日期**：2025 年 2 月 5 日

以下功能和改良功能將從 1 月版開始提供。

### 功能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>建立並使用視覺片段</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>視覺片段是預先定義的視覺區塊，可在多個電子郵件傳遞或內容範本中重複使用。此功能現已可供所有執行伺服器版本 8.6.4 及以上版本的客戶使用。</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>如需詳細資訊，請參閱<a href="../content/use-visual-fragments.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用第三方系統來傳送傳遞</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Campaign Web 介面中定義外部傳遞和外部傳遞範本。在此模式中，訊息會編譯成一個輸出檔案，該檔案可以與您的外部提供者共用。依據預設，外部傳遞模式是用於直接郵件管道。</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>如需詳細資訊，請參閱<a href="../msg/send-external-deliveries.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>管理您的列舉</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接透過 Adobe Campaign Web 使用者介面建立列舉。列舉是系統建議填入欄位的值清單。使用列舉來標準化這些欄位的值，以協助資料輸入或在查詢中使用。</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>如需詳細資訊，請參閱<a href="../administration/enumerations.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>建立自訂選項</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 使用者介面中存取技術選項，並建立自己的自訂選項來滿足您的需求。在使用 JavaScript 程式碼工作流程活動來儲存中間資料時，這特別有用。</p>
<img src="assets/do-not-localize/options.gif">
<p>如需詳細資訊，請參閱<a href="../administration/options.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>定義並呼叫 JavaScript 程式碼</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 使用者介面中建立 JavaScript 程式碼。這可讓您建立能夠跨工作流程使用的可重複使用函數，類似於程式庫。</p>
<img src="assets/do-not-localize/javascript.gif">
<p>如需詳細資訊，請參閱<a href="../administration/javascript-codes.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用 AI 助理產生登陸頁面</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>AI 助理現在可用於您的登陸頁面傳遞，讓您能夠產生文字、影像或完整的網頁版面。</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>如需有關 AI 助理的詳細資訊，請參閱<a href="../email/generative-lp.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>


### 改良功能 {#25-1-improvements}

* 自訂介面中自訂欄位的顯示：

   * 您現在可以選取要在介面中顯示的額外自訂欄位
   * 您現在可以設定用於顯示連結類型自訂欄位的規則，例如根據另一個欄位的輸入來限制清單值
   * 您現在可以更靈活地排列介面中的欄位：欄位可以跨越單一欄，或分組為子區段以便更好地組織
   * 您現在可以將特定欄位設定為唯讀

* 最近和我的最愛篩選器：為了快速重複使用常用的屬性，您現在可以將它們新增到我的最愛中。這可確保它們能夠輕鬆用於未來的任務中。除了我的最愛之外，您還可以檢視和使用最近選取的屬性。

* 外部帳戶：建立新的外部帳戶時，有全新&#x200B;**[!UICONTROL 路由]**&#x200B;類型可供選擇。此帳戶允許您設定一個特定的外部帳戶，可供外部傳遞使用。[了解更多](../administration/external-account.md#routing)
