---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 2026年3月發行 {#26-3-release}

### 新功能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>結構描述製作(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>結構描述製作功能現在可供所有客戶使用(GA)。 此功能可讓您直接從Campaign Web使用者介面建立和管理方案。 您可以建立新表格、擴充現有方案和建立自訂表單。 您可以定義自訂資料結構，以支援您的特定業務需求，而不需要存取使用者端主控台。</p>
<p>如需詳細資訊，請參閱<a href="../administration/schemas.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>電子郵件Designer (LA)中的主題</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>主題可讓您定義符合品牌指引的可重複使用主題樣式，以提供改良的電子郵件製作體驗。 您現在可以在片段中使用主題變數，確保電子郵件範本中的樣式一致。 此功能可讓您使用預先定義的模組更快速地建立電子郵件，這些模組會抽象化內容元素，例如標題、說明、影像和連結，同時維持品牌一致性。</p>
<p>注意：此功能目前僅開放給某些組織使用 (有限開放)，並將在未來版本中在全面推出。</p>
<p>如需詳細資訊，請參閱<a href="../email/apply-email-themes.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>整合自訂Firefly模型與協力廠商影像產生模型</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>可緊密整合標準與自訂Firefly模型，以及經核准的協力廠商影像模型，以便在產生影像時提供更大的彈性、控制力及品牌一致性。</p>
<p>選擇符合您需求的正確模式：</p>
<ul><li> <strong>Adobe模型</strong> （由Firefly Image Model 4提供技術支援）可立即產生影像，無需額外設定</li><li> <strong>合作夥伴機型</strong> （由Gemini 2.5 Flash提供），提供專門的功能</li><li><strong>自訂模型</strong> （在您自己的資產上訓練的品牌特定模型），用於品牌上產生，完全符合您的品牌識別、風格和視覺准則。</li></ul>
<p>如需詳細資訊，請參閱<a href="../content/generative-models.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自動化傳遞活動</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>工作流程浮動視窗中現在提供<strong>自動傳送</strong>工作流程活動。 您可以用它直接在您的工作流程中建立或執行傳遞動作（準備、傳送證明、準備和開始等）。 選取在工作流程之外建立的現有傳送，以在每次執行時重複使用它，或在每次活動執行時從範本建立新傳送。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/automated-delivery.md">詳細檔案。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>多個工作流程分支和加入活動</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>現在支援多個分支</strong>。 您可以按一下工具列上的[新增分支] <strong>，而不使用[分叉] </strong> <strong>。 </strong><strong>AND — 加入</strong>活動也已改善。 它現在是通用的<strong>加入</strong>活動，可讓您在AND和OR加入選項之間選擇。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>如需詳細資訊，請參閱<a href="../workflows/orchestrate-activities.md#toolbar">協調活動</a>和<a href="../workflows/activities/join.md">加入</a>檔案頁面。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-3-improvements}

* 已新增&#x200B;**開始**&#x200B;工作流程活動，以改善與使用者端主控台的相容性。 此活動為選用活動，預設不會插入新工作流程中。 不過，會自動新增至現有的工作流程。
  [了解更多](../workflows/activities/about-activities.md#flow-control)
* 傳遞的&#x200B;**排程**&#x200B;設定中的時區選取欄位已移動到&#x200B;**聯絡日期**&#x200B;欄位下方。 [了解更多](../msg/create-deliveries.md#gs-schedule)