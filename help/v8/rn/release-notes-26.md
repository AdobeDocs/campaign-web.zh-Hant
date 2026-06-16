---
title: Campaign v8 Web 使用者介面先前發行說明
description: 2026 Campaign Web 使用者介面版本
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: ed3fd4bbe8466c049af13304526daea948ab4706
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 97%

---

# 2026 年發行說明 {#2026-release}

此頁面列出了 **2026 年版本**&#x200B;的所有變更和改進。 最新的發行說明請前往[此頁面](release-notes.md)查閱。

## 2026 年 4 月版 {#26-4-release}

_2026 年 4 月 29 日_

### 改進 {#26-4-improvement}

「**擴充資料**」區段現已在「**建立客群**」工作流程活動 (查詢類型) 中提供。 您可以直接從 Campaign Web 使用者介面中檢視、新增、編輯及移除&#x200B;**附加資料**。 如同在「**擴充**」活動中一樣，您可以新增單一擴充屬性、集合連結和運算式。

[了解更多](../workflows/activities/build-audience.md)

## 2026 年 3 月發行版本 {#26-3-release}

_2026 年 3 月 24 日_

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

* 「**開始**」工作流程活動已新增，從而改善與用戶端控制台的相容性。此活動是選擇性的，依預設不會插入新的工作流程中。不過，它會自動新增至現有的工作流程。
  [了解更多](../workflows/activities/about-activities.md#flow-control)
* 傳遞的&#x200B;**排程**&#x200B;設定中的時區選取欄位已移動到&#x200B;**聯絡日期**&#x200B;欄位下方。 [了解更多](../msg/create-deliveries.md#gs-schedule)

## 2026 年 2 月版 {#26-2-release}

_2026 年 2 月 17 日_

### 新功能 {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>行銷活動詳細目錄中的時間軸視圖</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>行銷活動詳細目錄現在包含時間軸視圖，可以視覺化並管理一段時間內的行銷活動：在清單和時間軸之間切換、依週、月或日導覽、使用「今天」按鈕跳至目前日期，以及在右側面板中開啟行銷活動詳細資訊 (狀態、工作流程、傳送)，與清單視圖使用相同的篩選器和搜尋。</p>
<p>如需詳細資訊，請參閱<a href="../campaigns/manage-campaigns.md#timeline">詳細文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>結構描述編寫 (有限開放)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接在 Campaign Web 使用者介面中建立和管理結構描述。 此功能可以建立新表格、擴充現有結構描述和建立自訂表單。 您可以定義自訂資料結構，不需要存取用戶端主控台，便能支援特定業務需求。</p>
<p>注意：此功能目前僅開放給某些組織使用 (有限開放)，並將在未來版本中在全面推出。</p>
<p>如需詳細資訊，請參閱<a href="../administration/schemas.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## 2026 年 1 月版 {#26-1-release}

_2026 年 1 月 27 日_

### 新功能 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>多語言傳送功能 (正式推出)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>所有客戶現在都能使用多語言傳送功能(GA)。此功能可讓您在Adobe Campaign網頁使用者介面中，以不同語言傳送多則訊息。您可以選擇傳送的預設語言，以及傳送傳送時所使用的不同語言。您也可以使用所選的語言預覽這些傳送。 
<p>如需詳細資訊，請參閱<a href="../msg/multilingual.md">詳細文件</a>以瞭解詳情。</p>
<p>已為多語言推播通知進行下列改進：</p>
<ul>
<li>您現在可以上傳包含多語言內容的CSV檔案，快速填入所有語言變體。<a href="../msg/multilingual.md#csv-upload">瞭解詳情</a>
</li>
<li>現在支援富文字推播通知。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>交易型訊息中的輪廓擴充 (正式推出)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>現在所有客戶都可以使用「交易型訊息」功能中的設定檔擴充 (正式推出)。 除了電子郵件之外，現在也支援簡訊和推播通知。 此功能可以把 Adobe Campaign 資料庫欄位連結至訊息內容，個人化交易型訊息。 您可以選取目標對應、擴充欄和調和索引鍵，以確保準確且即時的個人化，同時維持績效臨界值。</p>
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/profile-enrichment.md">詳細文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager 即時和語言副本</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Manager 內容整合可以在建立傳遞內容時，直接在 Campaign 中存取在 Adobe Experience Manager 中建立的所有語言和即時副本。 您可以重新整理即時內容以擷取最新的 Adobe Experience Manager 版本。 此整合免除了 Adobe Experience Manager 與 Campaign 之間的內容手動同步，簡化多語言行銷活動工作流程。</p>
<p>如需詳細資訊，請參閱<a href="../integrations/aem-multilingual.md">詳細文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>內容實驗 - A/B 測試</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign Web 的內容實驗能定義多個 A/B 測試傳遞變化版本，測量哪些變化版本最適合您的目標客群。 您可以變更傳遞內容、主旨或寄件者，測試不同版本並判斷哪個變化版本能產生最佳結果。 您可以對不同電子郵件元素進行 A/B 測試，像是，主旨列、寄件者名稱和電子郵件內文內容。</p>
<p>如需詳細資訊，請參閱<a href="../email/ab-testing.md">詳細文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>持續傳遞活動</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>「持續傳遞」活動可以將新收件者新增至現有傳遞。 此傳遞類型不需要每次都建立新的傳遞，對於少量的警示或依需求傳送的通知而言，能大幅提升效率。 一個持續傳遞建立一個傳遞實例。 所有傳遞記錄 (broadLog) 和追蹤記錄都參考這個傳遞，藉此簡化監控和報告。</p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/continuous-delivery.md">詳細文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>行銷活動核准管理</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>核准程序有助於協調多個利害關係人，並在傳送前確認品質管控。 當您的組織需要來自不同團隊的驗證時 (例如行銷經理審閱內容或資料分析師驗證目標客群)，請使用核准。</p>
<p>如需詳細資訊，請參閱<a href="../campaigns/campaign-approvals.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-1-improvements}

* 動態報告現在支援推播通知和簡訊。 [了解更多](../reporting/dynamic-reporting/get-started-reporting.md)
* 預先定義的篩選器：新的「共用篩選器」選項可以向組織中的其他使用者提供預先定義的篩選器。 [了解更多](../get-started/predefined-filters.md#share-filter)
* 現在在使用內容範本時，可使用 Adobe Experience Manager 中已建立的個人化欄位，例如名稱、電子郵件、日期和地址。
* 內容品質評估現在會在品牌指南外，檢查易讀性、連貫性和有效性問題影響，找出不清楚的訊息、不一致的語調或結構性差距。 [了解更多](../content/brands-score.md)
