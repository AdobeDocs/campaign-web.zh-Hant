---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 64%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 頁面中列出了先前版本可用的變更和改進。

## 2025年10月發行 {#25-10-updates}

_2025 年 10 月 28 日_

<table>
<thead>
<tr>
<th><strong>交易型訊息、推播通知和簡訊的多語言功能 (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在 Adobe Campaign Web 使用者介面中，以不同語言傳送多則交易型訊息、推播通知和簡訊。多語言傳遞功能可讓您選擇傳遞的預設語言，以及可以傳送傳遞的不同語言。您也可以使用您選擇的語言來預覽這些傳遞。</p>
<p>注意：此功能目前僅開放給某些組織使用 (有限開放)，並將在未來版本中在全面推出。</p>
<p>如需詳細資訊，請參閱<a href="../msg/multilingual.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>交易型訊息中的輪廓擴充 (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>此功能可讓您將 Adobe Campaign 資料庫欄位連結至訊息內容，以便個人化交易型訊息。您可以選取目標對應、擴充欄和調和索引鍵，以確保準確且即時的個人化，同時維持績效臨界值。</p>
<p>注意：此功能目前僅開放給某些組織使用 (有限開放)，並將在未來版本中在全面推出。此功能目前僅適用於電子郵件。</p>
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/profile-enrichment.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>與Adobe GenStudio整合</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>為了提升行銷效率及維持品牌一致性，您現在可以將GenStudio for Performance Marketing體驗與Campaign緊密整合。 這可讓您運用GenStudio的AI支援內容建立作業以及Campaign的進階協調功能。<p>
<p>如需詳細資訊，請參閱<a href="../integrations/genstudio.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>電子郵件設計工具中的深色模式支援</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>電子郵件Designer現在提供切換到深色模式檢視的功能，您可以在此處額外定義特定自訂設定。 請注意，最終呈現取決於收件者的電子郵件使用者端，而且並非所有電子郵件使用者端都支援深色模式。</p>
<p>如需詳細資訊，請參閱<a href="../email/accessible-content.md#dark-mode">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### 功能改善 {#25-10-improvements}

* 在使用者端主控台中建立的傳遞中，**對象**&#x200B;區段現在會指出是否已為校訂目標定義動態條件。<!-- [Learn more](../msg/gs-deliveries.md#access)-->

* 您現在可以使用電子郵件Designer的條件式內容功能設定條件，在新的和舊版規則產生器之間切換。<!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* 您現在可以在收件者綱要的畫面定義中選取集合連結，例如購買。 這會透過專用索引標籤，在設定檔畫面上顯示相關資料。<!-- [Learn more](../administration/schemas.md#collection-lists)-->

* 身為Campaign管理員，您現在可以設定與Salesforce CRM和Microsoft Dynamics的連線。
  [了解更多](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

