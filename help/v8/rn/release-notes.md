---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。 我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，這些發行說明每月會更新多次。 請定期進行檢查。

## 2026年9月發行 {#26-9-release}

_2026年9月22日_

### 新功能 {#26-9-features}

<table>
<thead>
<tr>
<th><strong>LINE 管道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign現在支援<strong>LINE</strong>頻道，此為常用的立即訊息應用程式。 使用文字、影像或視訊內容，在獨立傳遞或工作流程中，連同您的其他頻道，建立並傳送LINE訊息。 <a href="../line/get-started-line.md">閱讀更多</a></p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-9-improvements}

* **側邊導覽存取**：管理員現在可以在側邊導覽中隱藏特定的功能表專案。 [閱讀更多](../administration/schemas-browse-access.md#screen-def)
* **其他核准型別**：除了內容和目標核准之外，您現在可以要求行銷活動傳遞的預算與傳遞開始核准。 [閱讀更多](../campaigns/campaign-approvals.md#configure-approvals)
* **以訪客為基礎的SMS目標定位**：訪客目標對應現在可用於SMS傳遞。 [閱讀更多](../sms/create-sms.md)
* **工作流程取消按鈕**：新的&#x200B;**取消**&#x200B;按鈕可讓您還原工作流程中未儲存的變更。 [閱讀更多](../workflows/orchestrate-activities.md#save-cancel)
* **重複資料刪除具有多個值**： **在值清單之後**&#x200B;選項現在支援多個屬性。 [閱讀更多](../workflows/activities/deduplication.md#deduplication-configuration)
* **行動目標對應**：您現在可以為行動應用程式目標建立目標對應。 [閱讀更多](../administration/target-mappings.md#create-mapping)
* **外部資料庫擴充**：您現在可以擴充&#x200B;**擴充**&#x200B;或&#x200B;**建立對象**&#x200B;活動中外部資料庫的資料。 [閱讀更多](../workflows/activities/enrichment.md#external-data)
* **檔案對象調解**：您現在可以設定在從檔案定位對象時，是否將收件者匯入資料庫。 [閱讀更多](../audience/file-audience.md#upload)
* **集合上的直接聯結**：直接從集合選取屬性時，您現在可以選擇如何建立條件：使用建議的預設選項、彙總函式或進階直接聯結。 [閱讀更多](../query/build-query.md#links)

