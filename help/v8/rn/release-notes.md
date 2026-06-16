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
source-git-commit: 6581a2d6ab44b711ed6aea6736d60f932a7ce315
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 45%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。 我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，這些發行說明每月會更新多次。 請定期進行檢查。

## 2026年6月發行 {#26-6-release}

_2026年6月16日_

### 功能改進 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* 您現在可以從任何清單畫面匯出資料，包括追蹤記錄。 尋找您的清單，然後按一下匯出按鈕。 匯出包含目前載入的列，並會考慮畫面上顯示的欄以及任何作用中的搜尋或篩選器。 [了解更多](../get-started/list-filters.md)

* **重複資料刪除**&#x200B;和&#x200B;**結束**&#x200B;工作流程活動現在支援多個入站轉變。 時間
有一個以上的入站轉變可用，請使用活動中的&#x200B;**集合以聯結**&#x200B;區段
屬性以選取要連線的轉變。 在以下頁面瞭解更多資訊： [重複資料刪除](../workflows/activities/deduplication.md)，

<!--
[End](../workflows/activities/end.md)
-->

* 進階引數現在顯示在&#x200B;**組建對象** （查詢型別）和&#x200B;**擴充**&#x200B;工作流程活動的&#x200B;**擴充資料**&#x200B;區段中。 這些引數可讓您微調擴充資料的建置方式，包括分組、重複資料刪除、主要金鑰處理和傳入事件資料。 [了解更多](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
