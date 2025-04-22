---
audience: end-user
title: 用於建立工作流程的主要原則
description: 了解使用 Adobe Campaign Web 的關鍵工作流程原則
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# 建立工作流程的主要原則 {#gs-workflow-creation}

透過 Adobe Campaign Web，您可以在視覺化畫布上建置工作流程以便設計跨管道流程，例如分段、行銷活動執行和檔案處理。

## 工作流程內部有什麼？ {#gs-workflow-inside}

呈現已規劃之流程的工作流程圖表。其會說明要執行的各種任務以及任務如何連結在一起。

![呈現工作及其連線的工作流程範例圖表](assets/workflow-example.png){zoomable="yes"}

每個工作流程都包含：

* **活動**：活動指要執行的任務。圖表上的圖示代表各種活動。每種活動都有特定屬性，以及和所有活動共通的屬性。

  在工作流程圖表中，一個特定活動可以產生多個任務，特別是存在迴圈或週期性動作時。

* **轉變**：轉變會將來源活動連結到目標活動並定義其序列。

* **工作表**：工作表包含轉變攜帶的所有資訊。每個工作流程會使用多個工作表。整個工作流程的生命週期皆可使用這些表格中的資料。

## 建立工作流程的關鍵步驟 {#gs-workflow-steps}

行銷活動提供兩種建立工作流程的方法：

1. 工作流程可以從&#x200B;**工作流程**&#x200B;選單建立為獨立的工作流程。

   ![建立獨立工作流程之介面的螢幕擷圖](assets/create-a-standalone-wf.png){zoomable="yes"}

1. 可以從行銷活動的&#x200B;**工作流程**&#x200B;標籤，直接在行銷活動內建立工作流程。工作流程若是包含在行銷活動中，會與其他所有行銷活動的工作流程一起執行，且會在行銷活動層級集合呈現相關報告量度。

   ![在行銷活動中建立工作流程之介面的螢幕擷圖](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

建立工作流程的關鍵步驟如下所示：

![呈現工作流程建立流程的圖表](assets/workflow-creation-process.png){zoomable="yes"}

以下區段詳細介紹了這些步驟：

1. [建立您的工作流程並定義其屬性](create-workflow.md)
1. [協調和配置活動](orchestrate-activities.md)
1. [配置您的工作流程進階設定](workflow-settings.md)
1. [啟動您的工作流程並監控其執行情況](start-monitor-workflows.md)