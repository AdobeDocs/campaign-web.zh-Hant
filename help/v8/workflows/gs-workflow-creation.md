---
audience: end-user
title: 使用 Adobe Campaign Web 建立工作流程
description: 了解如何使用 Adobe Campaign Web 建置工作流程
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 33%

---


# 用於建立工作流程的主要原則 {#gs-workflow-creation}

透過Campaign v8網路，您可以將工作流程建置到視覺畫布中，以設計跨管道流程，例如細分、行銷活動執行、檔案處理。

您可以從「工作流程」功能表，或直接在行銷活動中建立工作流程，作為獨立的工作流程，在此情況下，工作流程將連結至行銷活動，並與所有其他行銷活動的工作流程一起執行。

## 工作流程內含什麼？

工作流程圖表可呈現預期的情況。 它說明要執行的各種任務以及它們如何連結在一起。

![](assets/workflow-example.png)

每個工作流程內含：

* **活動**：活動是要執行的任務。 各種活動會以圖示呈現在圖表上。 每個活動都有特定的屬性和其他所有活動通用的屬性。

   在工作流程圖表中，一個特定活動可以產生多個任務，特別是當存在循環或週期性動作。

* **轉變**：轉換會將來源活動連結至目的地活動，並定義其順序。

* **工作表**：工作表包含轉變攜帶的所有資訊。每個工作流程會使用多個工作表。這些表格中傳送的資料可在整個工作流程生命週期中使用。

## 建立工作流程的主要步驟

建立工作流程的主要步驟如下所示：

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="銷售機會" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>建立工作流程</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="不常使用" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>協調活動</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="驗證" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>設定進階設定（選擇性）</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="開始和監視工作流程" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>開始和監視工作流程執行</strong></a>
</div>
<p>
</td>
</tr></table>