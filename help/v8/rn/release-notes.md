---
title: 最新發行說明
description: 探索 Campaign Web 使用者介面隨附的新增功能
source-git-commit: 21d856f9651f3a392ba9d927bc26082ce9759396
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 9%

---

# 發行說明 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="新增功能"
>abstract="Adobe Campaign的網頁使用者介面版本會在持續傳遞模式上運作，允許以更可縮放、分階段的方法進行功能部署。 發行說明每月更新數次。"
>
>"**March release is now live**, including Direct mail channel, the new Change data source workflow activity, and other improvements."


<!--Last update: **March 19, 2024**-->

Adobe Campaign的網頁使用者介面版本會在持續傳遞模式上運作，允許以更可縮放、分階段的方法進行功能部署。 因此，這些發行說明每月會更新好幾次。 請定期檢查。

>[!AVAILABILITY]
>
>此版本可供所有開始使用此版本的使用者使用 [Campaign （主控台） v8.6版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hant). 進一步瞭解Adobe Campaign使用者端主控台發行和升級，請參見 [Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hant){target="_blank"}.

## 3月發行 {#24-3-release}

**發行日期**： 2024年3月19至20日

### 直接郵件頻道 {#24-3-dm}

**直接郵件** 頻道現在可用於工作流程中，並作為獨立傳送。 直接郵件是一種離線頻道，可讓您建立、個人化和產生擷取檔案，並與直接郵件供應商共用以傳送郵件給您的客戶。 [深入了解](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 新的變更資料來源工作流程活動 {#24-3-change-data-source}

此 **變更資料來源** 目標定位活動可讓您變更工作流程工作表所使用的資料來源。 此活動可讓您跨不同的資料庫管理資料並改善效能，因此提供更大的彈性。 [深入了解](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 分割工作流程活動改善 {#24-3-split}

您現在可以使用 **在相同表格中產生所有子集** 中的選項 **Split** 工作流程活動，將所有子集分組為單一輸出轉變。 [深入了解](../workflows/activities/split.md)

### 查詢建模工具 {#24-3-query-modeler}

* 查詢模組化工具現在可用於電子郵件設計工具。 它可讓您在建立條件式內容時建置條件。 [深入了解](../personalization/conditions.md)
* 建立自訂條件時，預先定義的值現在可用於日期型別屬性。 [深入了解](../query/build-query.md)
* 在圖表的新轉變中無法再新增運運算元。 它們只能在篩選元件以將它們分組之前，新增到現有轉變上。 [深入了解](../query/build-query.md)
