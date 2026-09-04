---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 78%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。 我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，這些發行說明每月會更新多次。 請定期進行檢查。

## 2026月 8 月版本 {#26-8-release}

_2026 年 8 月 18 日_

### 新功能 {#26-8-features}

<table>
<thead>
<tr>
<th><strong>核准工作流程活動</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>核准</strong>工作流程活動 (先前僅在用戶端主控台中提供) 現在已於 Campaign Web 使用者介面中推出。 將任務指派給群組或個別操作者，自訂通知標題和訊息，並定義可能的答案 (例如「是／否」) 作為輸出分支。</p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/approval.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-8-improvements}

* **開啟追蹤**：您現在可以直接從 Campaign Web 使用者介面啟用或停用開啟追蹤。 這有助於您遵循資料保護法規。 [閱讀更多](../advanced-settings/delivery-settings.md#tracking-tab)
* **方案清單檢視**：方案現在會以專屬檢視列出，與行銷活動、即時傳遞和工作流程類似。 您可以從此檢視中瀏覽現有計畫並建立新方案。 [閱讀更多](../administration/plans-programs.md#create-program)
* **自訂結構描述設定**：在&#x200B;**動作資料**&#x200B;區段中，您現在可以禁止對自訂結構描述記錄執行&#x200B;**複製**&#x200B;動作。 [閱讀更多](../administration/schemas-action-data.md#action-data)
* **自訂篩選器**：在結構描述編輯器中，您現在可以使用新的&#x200B;**連結設定**&#x200B;對話方塊，限制連結型別自訂篩選器選擇器中可用的值。 [閱讀更多](../administration/schemas-custom-filters.md#settings)
* **結構描述驗證**：您現在可以使用新的&#x200B;**檢查**&#x200B;按鈕，直接從結構描述編輯器驗證結構描述的結構。 [閱讀更多](../administration/schemas-create-publish.md#create-new)
* **資料夾安全性**：資料夾上可用的動作現在會一致地受操作員的許可權控制，符合使用者端主控台的行為。 [了解更多](../get-started/work-with-folders.md#about-folders)。
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

