---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: ht
source-wordcount: '770'
ht-degree: 100%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[此頁面](release-notes-24.md)列出先前版本可用的變更和改良功能。

## 2025 年 2 月發行版本 {#25-2-release}

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