---
title: Campaign v8 Web 使用者介面早期發行說明
description: 探索下一個 Campaign Web 使用者介面版本的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 100%

---

# 早期發行說明 {#e-release}

Adobe Campaign Web 使用者介面持續提供新功能、現有功能的增強功能並修正錯誤。所有變更都會在每個月月末整合於[發行說明](release-notes.md)中。

**在發行日期之前，以下早期發行說明如有更改，恕不另行通知**。連結、畫面和更新文件會於發行日期在[發行說明](release-notes.md)中發佈。

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
<p>您現在可以在 Campaign Web 介面中定義外部傳遞和外部傳遞範本。在此模式中，訊息會編譯成一個輸入檔案，該檔案可以與您的外部提供者共用。依據預設，外部傳遞模式是用於直接郵件管道。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>建立業務規則 (類型規則)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 介面中建立類型和類型規則。類型是類型規則的集合，可協助控制、篩選傳遞並排定其優先順序。類型可確保您的傳遞始終包含必要元素 (例如取消訂閱連結或主旨列)，並套用篩選規則以從您的目標客群中排除特定群組 (例如取消訂閱者、競爭者或非忠誠客戶)。</p>
<img src="assets/do-not-localize/typology.gif">
<p>如需詳細資訊，請參閱<a href="../administration/typologies.md">詳細說明文件</a>。</p>
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

### 改良功能 {#25-1-improvements}

* 自訂介面中自訂欄位的顯示：

   * 您現在可以選取要在介面中顯示的額外自訂欄位
   * 您現在可以設定用於顯示連結類型自訂欄位的規則，例如根據另一個欄位的輸入來限制清單值
   * 您現在可以更靈活地排列介面中的欄位：欄位可以跨越單一欄，或分組為子區段以便更好地組織
   * 您現在可以將特定欄位設定為唯讀

* 最近和我的最愛篩選器：為了快速重複使用常用的屬性，您現在可以將它們新增到我的最愛中。這可確保它們能夠輕鬆用於未來的任務中。除了我的最愛之外，您還可以檢視和使用最近選取的屬性。


