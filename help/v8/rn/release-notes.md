---
title: 最新發行說明
description: 探索 Campaign Web 使用者介面隨附的新增功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: ht
source-wordcount: '342'
ht-degree: 100%

---

# 發行說明 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="新增功能"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，通過該模型可採用更具擴充性、分階段的方式部署功能。發行說明每月會多次更新。**3 月版本現已上線**，包括直接郵件頻道、新的變更資料來源工作流程活動以及其他改善事項。"


<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，通過該模型可採用更具擴充性、分階段的方式部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

>[!AVAILABILITY]
>
>此版本適用於從 [Campaign (控制台) v8.6 發行版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hant)開始的所有使用者。 請參閱 [Campaign v8 (控制台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hant){target="_blank"}，了解更多有關 Adob&#x200B;&#x200B;e Campaign 客戶端控制台發行版本和升級。

## 3 月發行說明 {#24-3-release}

**發行日期**：2024 年 3 月 19-20 日

### 直接郵件頻道 {#24-3-dm}

**直接郵件**&#x200B;頻道現已可在工作流程中使用，並可作為獨立傳遞來使用。直接郵件是離線頻道，可讓您建立、個人化和產生摘取檔案，並將該檔案與您的直接郵件提供者分享，以便他們傳送郵件給您的客戶。[閱讀更多](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 新的變更資料來源工作流程活動 {#24-3-change-data-source}

新的&#x200B;**變更資料來源**&#x200B;目標定位活動可讓您變更工作流程工作表格使用的資料來源。 此活動可讓您跨不同的資料庫管理資料，為您提供更多彈性並改善工作效率。[閱讀更多](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 分割工作流程活動的改善 {#24-3-split}

現在您可以使用「**分割**」工作流程活動中的「**在相同表格中產生所有子集**」選項，將所有子集歸類至單一的輸出轉換。[閱讀更多](../workflows/activities/split.md)

### 查詢建模工具 {#24-3-query-modeler}

* 查詢建模工具現在可在電子郵件設計工具中使用。此工具可讓您在建立條件內容時建立條件。[閱讀更多](../personalization/conditions.md)
* 建立自訂條件時，預定義值現在適用於日期類型屬性。[閱讀更多](../query/build-query.md)
* 無法再於圖中的新轉換上新增運算子。這些運算子只能先新增在現有的轉換中，然後才能篩選組件並歸類在一起。[閱讀更多](../query/build-query.md)
