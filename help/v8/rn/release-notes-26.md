---
title: Campaign v8 Web 使用者介面先前發行說明
description: 2026 Campaign Web 使用者介面版本
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 23%

---

# 2026 年發行說明 {#2026-release}

此頁面列出了 **2026 年版本**&#x200B;的所有變更和改進。[此頁面](release-notes.md)提供最新發行說明。

## 2026年2月發行 {#26-2-release}

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
<th><strong>行銷活動詳細目錄中的時間表檢視</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>行銷活動詳細目錄現在包含時間軸檢視，可讓您隨著時間視覺化和管理行銷活動：在清單和時間軸之間切換、依周、月或日導覽、使用「今天」按鈕跳至目前日期，以及在右側面板中開啟行銷活動詳細資訊（狀態、工作流程、傳送），且篩選器和搜尋與清單檢視相同。</p>
<p>如需詳細資訊，請參閱<a href="../campaigns/manage-campaigns.md#timeline">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>結構描述製作(LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接從Campaign網頁使用者介面建立和管理方案。 此功能可讓您建立新表格、擴充現有方案和建立自訂表單。 您可以定義自訂資料結構，以支援您的特定業務需求，而不需要存取使用者端主控台。</p>
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

## 2026年1月發行 {#26-1-release}

_2026 年 1 月 27 日_

### 新功能 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>多語言傳送功能(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>所有客戶現在都能使用多語言傳送功能(GA)。 此功能可讓您在Adobe Campaign網頁使用者介面中，以不同語言傳送多則訊息。 您可以選擇傳送的預設語言，以及傳送傳送時所使用的不同語言。 您也可以使用您選擇的語言來預覽這些傳遞。 
<p>如需詳細資訊，請參閱<a href="../msg/multilingual.md">詳細文件</a>以瞭解詳情。</p>
<p>已針對多語言推播通知進行下列改良：</p>
<ul>
<li>您現在可以上傳包含多語言內容的CSV檔案，快速填入所有語言變體。 <a href="../msg/multilingual.md#csv-upload">閱讀更多</a>
</li>
<li>現在支援豐富推送通知。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>異動訊息(GA)中的設定檔擴充</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>現在所有客戶都可以使用「異動訊息」功能中的設定檔擴充(GA)。 除了電子郵件之外，現在也支援簡訊和推播通知。 此功能可讓您將Adobe Campaign資料庫欄位連結至訊息內容，以個人化交易式訊息。 您可以選取目標對應、擴充欄和調和索引鍵，以確保準確且即時的個人化，同時維持績效臨界值。</p>
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/profile-enrichment.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager即時和語言副本</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Manager內容整合可讓您在建立傳遞內容時，直接在Campaign中存取在Adobe Experience Manager中建立的所有語言和即時副本。 您可以即時重新整理內容以擷取最新的Adobe Experience Manager版本。 此整合可避免Adobe Experience Manager與Campaign之間的手動內容同步，簡化您的多語言行銷活動工作流程。</p>
<p>如需詳細資訊，請參閱<a href="../integrations/aem-multilingual.md">詳細文件</a>以瞭解詳情。</p>
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
<p>Adobe Campaign網站中的內容實驗可讓您定義多個A/B測試傳送變體，以測量哪些變體最適合您的目標對象。 您可以變更傳遞內容、主旨或寄件者，以測試不同版本並判斷哪個變體產生最佳結果。 您可以對各種電子郵件元素進行A/B測試，例如主旨列、寄件者名稱和電子郵件內文內容。</p>
<p>如需詳細資訊，請參閱<a href="../email/ab-testing.md">詳細文件</a>以瞭解詳情。</p>
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
<p>「持續傳遞」活動可讓您將新收件者新增至現有傳遞。 此傳送型別可避免每次都必須建立新傳送，因此可更有效地視需要傳送低流量警報或通知。 持續傳遞會建立單一傳遞執行個體。 所有傳遞記錄(broadLog)和追蹤記錄都參考這個傳遞，藉此簡化監控和報告。</p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/continuous-delivery.md">詳細文件</a>以瞭解詳情。</p>
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
<p>核准程式可協助協調多個利害關係人，並確保在傳送前進行品質控制。 當您的組織需要來自不同團隊的驗證時（例如行銷經理稽核內容或資料分析師驗證目標對象），請使用核准。</p>
<p>如需詳細資訊，請參閱<a href="../campaigns/campaign-approvals.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-1-improvements}

* 動態報告現在支援推播通知和SMS。 [了解更多](../reporting/dynamic-reporting/get-started-reporting.md)
* 預先定義的篩選器 — 新的「共用篩選器」選項可讓您為組織中的其他使用者提供預先定義的篩選器。 [了解更多](../get-started/predefined-filters.md#share-filter)
* 現在包含在Adobe Experience Manager中建立的個人化欄位，例如名稱、電子郵件、日期和地址，而且可在使用內容範本時使用這些欄位。
* 內容品質評估現在會檢查可讀性、連貫性和有效性問題，而不受品牌指南的影響，找出不清楚的訊息、不一致的語調或結構性差距。 [了解更多](../content/brands-score.md)
