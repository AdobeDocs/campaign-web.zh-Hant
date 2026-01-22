---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ca1a437f8a8a25c0a15b9148e9c73271795f16c7
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 頁面中列出了先前版本可用的變更和改進。

## 2025 年 10 月發行版本 {#25-10-updates}

_2025 年 11 月 3 日_

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
<p>如需詳細資訊，請參閱<a href="../msg/multilingual.md">詳細文件</a>以瞭解詳情。</p>
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
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/profile-enrichment.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>與 Adobe GenStudio 整合</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以將 GenStudio for Performance Marketing 體驗與 Campaign 緊密整合，以便提高行銷效率及維持品牌一致性。藉由這樣的整合，您便可以搭配 Campaign 的進階協調功能，使用 GenStudio 由 AI 驅動的內容創作。<p>
<p>如需詳細資訊，請參閱<a href="../integrations/genstudio.md">詳細文件</a>以瞭解詳情。</p>
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
<p>電子郵件設計工具現在可以切換成深色模式的視圖，而且您可以在這裡定義其他特定的自訂設定。請注意，最終轉譯的結果取決於收件者的電子郵件用戶端，而並非所有電子郵件用戶端都支援深色模式。</p>
<p>如需詳細資訊，請參閱<a href="../email/dark-mode.md">詳細文件</a>以瞭解詳情。</p>
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

### 功能改進 {#25-10-improvements}

* 在用戶端控制台所建立的傳遞中，**客群**&#x200B;區段現在會指出是否已經定義校訂目標的動態條件。<!-- [Learn more](../msg/gs-deliveries.md#access)-->

* 現在，您使用電子郵件設計工具的條件式內容功能來設定條件時，可以在新版和舊版規則產生器之間切換。<!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* 您現在可以在收件者結構描述的畫面定義中選取集合連結，例如購買。這樣做會透過專用的索引標籤，在輪廓畫面上顯示相關資料。<!-- [Learn more](../administration/schemas.md#collection-lists)-->

* 身為 Campaign 管理員，您現在可以設定與 Salesforce CRM 和 Microsoft Dynamics 的連線。
  [了解更多](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

