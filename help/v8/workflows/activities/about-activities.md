---
audience: end-user
title: 使用工作流程活動
description: 了解如何使用工作流程活動
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 35%

---


# 關於工作流程活動 {#workflow-activities}

工作流程活動可歸類為三個類別。可用的活動可能會依據內容而有所不同。

以下各節會詳細介紹所有活動：

* [目標定位和資料管理活動](#targeting)
* [管道活動](#channel)
* [流程控制活動](#flow-control)

![](../assets/workflow-activities.png)

## 目標定位和資料管理活動 {#targeting}

這些活動專門針對目標定位、操控和擴充母體資料。這些活動可讓您使用交集、聯合或排除作業定義對象並分割或結合這些對象，從而建置一個或多個目標。

* 使用 [儲存對象](save-audience.md) 活動，以更新現有的對象，或從工作流程中的母體運算上游建立新的對象。
* 使用 [建立對象](build-audience.md) 定義目標母體的活動。 您可以選取現有對象，或使用查詢建模器來定義您自己的查詢。
* 使用 [合併](combine.md) 活動，對傳入母體執行分段。 您可以使用聯合、交集或排除。
* 使用 [Split](split.md) 將傳入母體分段為數個子集的活動。
* 使用 [調解](reconciliation.md) 活動定義Adobe Campaign資料庫中的資料與工作表中的資料（例如從外部檔案載入的資料）之間的連結。
* 使用 [擴充](enrichment.md) 活動，定義要在工作流程中處理的其他資料。 透過此活動，您可以利用傳入轉變並設定活動，以使用其他資料完成傳出轉變。
* 使用 [重複資料刪除](deduplication.md) 活動以刪除入站活動結果中的重複專案。
* 使用 [變更維度](change-dimension.md) 活動，以在您建置工作流程時變更目標維度。
* 使用 [載入檔案](load-file.md) 使用儲存在外部檔案中的設定檔和資料的活動。

## 管道活動 {#channel}

Adobe Campaign Web可讓您跨多個管道自動執行行銷活動。 您可以將管道活動結合到畫布中，以建立跨管道工作流程，其可以根據客戶行為觸發動作。 下列專案 **頻道** 提供活動：電子郵件、簡訊、Android和iOS推播通知。 [瞭解如何在工作流程內容中設定傳送](channels.md).

## 流程控制活動 {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="結束活動"
>abstract="「**結束**」活動可讓您以圖形方式標記工作流程的終點。此活動並不會造成任何功能性影響，因此為選用。"

下列活動僅限於整理和執行工作流程。這些活動的主要任務是協調其他活動：

* 使用 [排程器](scheduler.md) 排程工作流程開始時間的活動。
* 使用 [合併連結](and-join.md) 同步工作流程多個執行分支的活動。
* 新增 **結束** 活動，以圖形方式標示工作流程的結尾。 此活動並不會造成任何功能性影響，因此為選用。
* 使用 [分支](fork.md) 活動，用來建立出站轉變，以同時啟動多個活動。
* 新增 [等待](wait.md) 活動可暫時暫停執行工作流程的一部分。

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

