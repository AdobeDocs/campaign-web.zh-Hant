---
audience: end-user
title: 使用 Adobe Campaign Web 建立工作流程
description: 了解如何使用 Adobe Campaign Web 建置工作流程
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 57%

---


# 用於建立工作流程的主要原則 {#gs-workflow-creation}

透過 Campaign v8 Web，您可以將工作流程建置到視覺化畫布中，以設計跨管道流程，例如分段、行銷活動執行、檔案處理。


## 工作流程內部有什麼？ {#gs-workflow-inside}

工作流程圖表代表應該發生的情況。它會說明要執行的各種任務以及任務如何連結在一起。

![](assets/workflow-example.png)

每個工作流程都包含：

* **活動**：活動指要執行的任務。各種活動在圖表中會以圖示表示。每種活動都有特定屬性和所有活動共有的其他屬性。

  在工作流程圖表中，一個特定活動可以產生多個任務，尤其是存在迴圈或週期性動作時。

* **轉變**：轉變會將來源活動連結到目標活動並定義其序列。

* **工作表**：工作表包含轉變攜帶的所有資訊。每個工作流程會使用多個工作表。這些表格中傳送的資料可在整個工作流程生命週期中使用。

## 建立工作流程的關鍵步驟 {#gs-workflow-steps}


行銷活動提供兩種建立工作流程的方式：

1. 工作流程可以建立為獨立的工作流程，從 **工作流程** 功能表。

   ![](assets/create-a-standalone-wf.png)

1. 工作流程可直接在行銷活動中建立，從 **工作流程** 行銷活動的索引標籤。 納入行銷活動時，工作流程會與其他所有行銷活動的工作流程一起執行，而報告量度都會在行銷活動層級分組。

   ![](assets/create-a-wf-from-a-campaign.png)


建立工作流程的關鍵步驟如下：

![](assets/workflow-creation-process.png)

以下章節將詳細介紹這些步驟：

1. [建立您的工作流程並定義其屬性](create-workflow.md)
1. [協調與設定活動](orchestrate-activities.md)
1. [設定工作流程進階設定](workflow-settings.md)
1. [開始您的工作流程並監視其執行](start-monitor-workflows.md)

