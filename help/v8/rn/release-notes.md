---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 91%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。 我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，這些發行說明每月會更新多次。 請定期進行檢查。

## 2026年4月發行 {#26-4-release}

_2026年4月29日_

### 改進 {#26-4-improvement}

**擴充資料**&#x200B;區段現在可在&#x200B;**建置對象**&#x200B;工作流程活動（查詢型別）中使用。 您可以直接從Campaign網頁使用者介面檢視、新增、編輯及移除&#x200B;**其他資料**。 如同在&#x200B;**擴充**&#x200B;活動中，您可以新增單一擴充屬性、集合連結和運算式。

[了解更多](../workflows/activities/build-audience.md)

## 2026 年 3 月發行版本 {#26-3-release}

_2026年3月_ 24日_

### 新功能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>結構描述編寫 (正式推出)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>結構描述編寫功能現在可供所有客戶使用 (正式推出)。 此功能可以直接在 Campaign Web 使用者介面中建立和管理結構描述。 您可以建立新表格、擴充現有結構描述和建立自訂表單。 您可以定義自訂資料結構，不需要存取用戶端主控台，便能支援特定業務需求。</p>
<p>如需詳細資訊，請參閱<a href="../administration/schemas.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>電子郵件設計工具中的主題 (限制性開放)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>主題可以重複使用符合品牌指引的主題風格，改善電子郵件的製作體驗。 您現在可以在片段中使用主題變數，確保電子郵件範本中的風格一致。 此功能可讓您使用預先定義的模組更快速地建立電子郵件，這些模組可以摘要內容元素，例如標題、說明、影像和連結，同時維持品牌一致性。</p>
<p>注意：此功能目前僅開放給某些組織使用 (有限開放)，並將在未來版本中在全面推出。</p>
<p>如需詳細資訊，請參閱<a href="../email/apply-email-themes.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>整合自訂 Firefly 模型和第三方影像生成模型</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>啟用標準與自訂 Firefly 模型，以及經核准的第三方影像模型的緊密整合，以便在生成影像時提供更大的彈性、控制力及品牌一致性。</p>
<p>選擇符合您需求的正確模型：</p>
<ul><li> <strong>Adobe 模型</strong> (由 Firefly Image Model 4 提供技術支援) 可立即產生影像，無需額外設定</li><li> <strong>合作夥伴模型</strong> (由 Gemini 2.5 Flash 提供)，提供專門的功能</li><li><strong>自訂模型</strong> (在您自己的資產上訓練的品牌特定模型)，用於品牌產生，完全符合您的品牌識別、風格和視覺指引。</li></ul>
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
<p>工作流程浮動面板現已提供<strong>自動化傳遞</strong>工作流程活動。 您可以使用此功能，直接在工作流程中建立或執行傳遞動作 (準備、傳送校訂、準備並開始等) 。 選取在工作流程外建立的重複執行使用的現有傳遞，或在每次活動執行時從範本建立新的傳遞。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/automated-delivery.md">詳細文件。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>多個工作流程分支和「加入」活動</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>現已支援<strong>多個分支</strong>。 您可以在工具列按一下<strong>新增分支</strong>，無需使用<strong>分岔</strong>。 <strong>AND-連接</strong>活動同樣已改進。 它現在是通用的<strong>連接</strong>活動，可讓您在「AND」和「OR」加入選項之間選擇。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>如需詳細資訊，請參閱<a href="../workflows/orchestrate-activities.md#toolbar">協調活動</a>和<a href="../workflows/activities/join.md">連接</a>檔案頁面。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-3-improvements}

* 已新增&#x200B;**開始**&#x200B;工作流程活動，以改善與用戶端主控台的相容性。 此活動為選用，預設不會插入新工作流程中。 不過，會自動新增至現有的工作流程。
  [了解更多](../workflows/activities/about-activities.md#flow-control)
* 傳遞的&#x200B;**排程**&#x200B;設定中的時區選取欄位已移動到&#x200B;**聯絡日期**&#x200B;欄位下方。 [了解更多](../msg/create-deliveries.md#gs-schedule)