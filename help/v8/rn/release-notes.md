---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 56%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign的網頁使用者介面版本會在持續傳遞模式上運作，允許以可縮放、分階段的方法進行功能部署。 因此，這些發行說明每月會更新數次。 請定期檢查。

舊版可用的變更和改進專案列於本頁](release-notes-24.md)的[中。

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
<p>您現在可以在 Adobe Campaign Web 使用者介面中建立類型和類型規則。型別可控制、篩選傳遞內容，並安排傳遞內容的優先順序。 型別可驗證傳遞一律包含必要元件（例如取消訂閱連結或主旨列）或篩選規則，以從您的對象中排除群組（例如取消訂閱者、競爭者或不忠誠客戶）。</p>
<img src="assets/do-not-localize/typology.gif" alt="在Adobe Campaign網路使用者介面中建立型別規則的圖例">
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
<p>現在您可以在 Campaign Web 使用者介面中建立目標對應。目標對應定義了不同的傳遞管道 (電子郵件、簡訊、推播通知) 如何連結到結構描述的資料欄位。目標對應會定義目標對象：設定檔、合約受益人、操作者、訂閱者、潛在客戶等。</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="在Adobe Campaign Web使用者介面中建立目標對應的圖例">
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
<p>現在您可以在清單中選取結構描述的名稱來存取其詳細資料。自訂欄位編輯現在可以從結構描述詳細資料中可用的<b>編輯自訂欄位</b>按鈕存取。</p>
<img src="assets/do-not-localize/schemas.gif" alt="在Adobe Campaign網頁使用者介面中編輯的結構描述詳細資料和自訂欄位的圖例">
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
<p>視覺片段是預先定義的視覺化區塊，您可以在多個電子郵件傳遞或內容範本中重複使用。 此功能現已可供所有執行伺服器版本 8.6.4 及以上版本的客戶使用。</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Adobe Campaign Web使用者介面中視覺片段建立與使用的圖示">
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
<img src="assets/do-not-localize/external-delivery.gif" alt="Adobe Campaign網頁使用者介面中的外部傳遞設定圖例">
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
<p>您現在可以直接透過 Adobe Campaign Web 使用者介面建立列舉。列舉是系統建議填入欄位的值清單。使用列舉來標準化這些欄位的值，協助資料輸入或在查詢中使用。</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Adobe Campaign Web使用者介面中的分項清單管理圖例">
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
<img src="assets/do-not-localize/options.gif" alt="在Adobe Campaign網頁使用者介面中建立自訂選項的圖例">
<p>如需詳細資訊，請參閱<a href="../administration/options.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>定義和呼叫JavaScript程式碼</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 使用者介面中建立 JavaScript 程式碼。這可讓您建立可重複使用的功能，這些功能可在類似程式庫的工作流程中使用。</p>
<img src="assets/do-not-localize/javascript.gif" alt="在JavaScript Web使用者介面中建立Adobe Campaign程式碼的圖例">
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
<img src="assets/do-not-localize/ai-lp.gif" alt="AI助理在Adobe Campaign網路使用者介面中用於產生登陸頁面的圖例">
<p>如需有關 AI 助理的詳細資訊，請參閱<a href="../email/generative-lp.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改良功能 {#25-1-improvements}

* 自訂介面中自訂欄位的顯示：
   * 選取其他自訂欄位以顯示於介面中。
   * 設定顯示連結型別自訂欄位的規則，例如根據其他欄位的輸入限制清單值。
   * 更靈活地排列介面中的欄位：欄位可以跨越單一欄，或分組到子區段中，以更好地進行組織。
   * 將特定欄位設定為唯讀。

* 最近和我的最愛篩選器：將常用的屬性新增到我的最愛，以便快速存取。 除了我的最愛之外，還可以檢視和使用最近選取的屬性。

* 外部帳戶：建立新的外部帳戶時，有全新&#x200B;**[!UICONTROL 路由]**&#x200B;類型可供選擇。此帳戶允許您設定一個特定的外部帳戶，可供外部傳遞使用。[了解更多](../administration/external-account.md#routing)。