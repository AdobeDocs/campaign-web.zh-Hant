---
title: Campaign v8 Web 使用者介面早期發行說明
description: 探索下一個 Campaign Web 使用者介面版本的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 126ebed5066bbc8c20d58d24e237b13f096b9d02
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 32%

---

# 早期發行說明 {#e-release}

Adobe Campaign Web 使用者介面持續提供新功能、現有功能的增強功能並修正錯誤。所有變更都會在每個月月末整合於[發行說明](release-notes.md)中。

**在發行日期之前，以下早期發行說明如有更改，恕不另行通知**。連結、畫面和更新文件會於發行日期在[發行說明](release-notes.md)中發佈。

## 2025年1月發行 {#25-1-release}

**發行日期**：2025年2月5日

從1月發行版本開始，將推出下列功能和改善專案。

### 功能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>建立及使用視覺片段</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>視覺片段是預先定義的視覺化區塊，您可以在多個電子郵件傳遞或內容範本中重複使用。 此功能現在可供所有在伺服器版本編號8.6.4及更高版本上執行的客戶使用。</p>
<p>如需詳細資訊，請參閱<a href="../content/use-visual-fragments.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用協力廠商系統來傳送傳遞</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在Campaign網頁使用者介面中定義外部傳遞和外部傳遞範本。 透過此模式，訊息將在輸入檔案中產生，該檔案可以與您的外部提供者共用。外部傳遞模式是直接郵件管道的預設模式。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>控制和篩選包含型別的傳遞傳送</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在Adobe Campaign網頁使用者介面中建立型別與型別規則。 類型是類型規則的集合，可讓您控制、篩選傳遞的傳送並排定其優先順序。型別驗證您的傳送一律包含必要元素（例如取消訂閱連結或主旨列），或篩選規則以將群組從您的預定目標中排除（例如取消訂閱者、競爭者或不忠誠客戶）。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>管理您的分項清單</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接透過Adobe Campaign網頁使用者介面建立分項清單。 分項清單是系統建議用來填入欄位的值清單。 使用列舉來標準化這些欄位的值，有助於資料輸入或在查詢中使用。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
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
<p>您現在可以存取Adobe Campaign網頁使用者介面中的技術選項，並建立自己的自訂選項以符合您的需求。 這在使用JavaScript程式碼工作流程活動來儲存中繼資料時特別有用。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>定義並呼叫Javascript程式碼</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在Adobe Campaign網頁使用者介面中建立JavaScript程式碼。 這可讓您建立可重複使用的功能，以便跨工作流程使用，類似資料庫。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改良功能 {#25-1-improvements}

* 自訂介面中自訂欄位的顯示：

   * 您現在可以選取要在介面中顯示的其他自訂欄位
   * 您現在可以設定顯示連結型別自訂欄位的規則，例如根據其他欄位的輸入限制清單值
   * 您現在可以更靈活地排列介面中的欄位：欄位可以跨越單一欄，或分組到子區段中以便更好地組織
   * 您現在可以將特定欄位設定為唯讀。

* 最近使用的和我的最愛篩選器：若要快速重複使用常用的屬性，您現在可以將它們新增到我的最愛。 這可確保可供未來任務隨時存取。 除了我的最愛之外，您還可以檢視和使用最近選取的屬性。


