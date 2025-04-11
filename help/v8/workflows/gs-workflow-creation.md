---
audience: end-user
title: 用於建立工作流程的主要原則
description: 了解使用 Adobe Campaign Web 的關鍵工作流程原則
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 41%

---

# 用於建立工作流程的主要原則 {#gs-workflow-creation}

透過Adobe Campaign Web，您可以在視覺畫布上建立工作流程，以設計跨管道流程，例如細分、行銷活動執行和檔案處理。

## 工作流程內部有什麼？ {#gs-workflow-inside}

工作流程圖表代表計畫流程。 它會說明要執行的各種任務以及任務如何連結在一起。

![工作流程範例圖表，顯示任務及其連線](assets/workflow-example.png){zoomable="yes"}

每個工作流程都包含：

* **活動**：活動指要執行的任務。圖表上的圖示代表各種活動。 每個活動都有所有活動通用的特定屬性和屬性。

  在工作流程圖表中，特定活動可產生多個任務，尤其是當有回圈或重複動作時。

* **轉變**：轉變會將來源活動連結到目標活動並定義其序列。

* **工作表**：工作表包含轉變攜帶的所有資訊。每個工作流程會使用多個工作表。這些表格中的資料可在工作流程的整個生命週期中使用。

## 建立工作流程的關鍵步驟 {#gs-workflow-steps}

行銷活動提供兩種建立工作流程的方法：

1. 可從&#x200B;**工作流程**&#x200B;功能表將工作流程建立為獨立的工作流程。

   ![建立獨立工作流程的介面熒幕擷圖](assets/create-a-standalone-wf.png){zoomable="yes"}

1. 可以從行銷活動的&#x200B;**工作流程**&#x200B;索引標籤，直接在行銷活動中建立工作流程。 將工作流程納入行銷活動時，會與其他所有行銷活動的工作流程一起執行，且報表量度會依行銷活動層級分組。

   ![在行銷活動中建立工作流程的介面熒幕擷圖](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

建立工作流程的關鍵步驟如下所示：

![顯示工作流程建立程式的圖表](assets/workflow-creation-process.png){zoomable="yes"}

以下各節將詳細介紹這些步驟：

1. [建立您的工作流程並定義其屬性](create-workflow.md)
1. [協調和配置活動](orchestrate-activities.md)
1. [配置您的工作流程進階設定](workflow-settings.md)
1. [啟動您的工作流程並監控其執行情況](start-monitor-workflows.md)