---
title: Campaign v8 Web 使用者介面先前發行說明
description: 2026 Campaign Web 使用者介面版本
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: ht
source-wordcount: '753'
ht-degree: 100%

---

# 2026 年發行說明 {#2026-release}

此頁面列出了 **2026 年版本**&#x200B;的所有變更和改進。最新的發行說明請前往[此頁面](release-notes.md)查閱。

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
<p>所有客戶現在都能使用多語言傳送功能 (正式推出)。此功能可以在 Adobe Campaign 網頁使用者介面中，以不同語言傳送多則訊息。多語言傳遞功能可選擇傳遞的預設語言，並以不同語言傳送傳遞。 您也可以使用您選擇的語言來預覽這些傳遞。 
<p>如需詳細資訊，請參閱<a href="../msg/multilingual.md">詳細文件</a>以瞭解詳情。</p>
<p>已為多語言推播通知進行下列改進：</p>
<ul>
<li>您現在可以上傳多語言內容的 CSV 檔案，快速填入您的所有語言變體。<a href="../msg/multilingual.md#csv-upload">閱讀更多</a>
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
<p>現在所有客戶都可以使用「交易型訊息」功能中的設定檔擴充 (正式推出)。除了電子郵件之外，現在也支援簡訊和推播通知。 此功能可以把 Adobe Campaign 資料庫欄位連結至訊息內容，個人化交易型訊息。 您可以選取目標對應、擴充欄和調和索引鍵，以確保準確且即時的個人化，同時維持績效臨界值。</p>
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
<p>Adobe Experience Manager 內容整合可以在建立傳遞內容時，直接在 Campaign 中存取在 Adobe Experience Manager 中建立的所有語言和即時副本。您可以重新整理即時內容以擷取最新的 Adobe Experience Manager 版本。 此整合免除了 Adobe Experience Manager 與 Campaign 之間的內容手動同步，簡化多語言行銷活動工作流程。</p>
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
<p>「持續傳遞」活動可以將新收件者新增至現有傳遞。此傳遞類型不需要每次都建立新的傳遞，對於少量的警示或依需求傳送的通知而言，能大幅提升效率。 一個持續傳遞建立一個傳遞實例。 所有傳遞記錄 (broadLog) 和追蹤記錄都參考這個傳遞，藉此簡化監控和報告。</p>
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
