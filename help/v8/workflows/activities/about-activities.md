---
audience: end-user
title: '使用工作流程活動 '
description: 了解如何使用工作流程活動
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 61f3a2bff32bba1e202d3e811e9f116f3987c191
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 20%

---

# 關於工作流程活動 {#workflow-activities}

工作流程活動可歸類為三個類別。可用的活動可能會依據內容而有所不同。

以下各節會詳細介紹所有活動：

* [目標定位和資料管理活動](#targeting)
* [管道活動](#channel)
* [流程控制活動](#flow-control)

![工作流程活動概觀](../assets/workflow-activities.png)

## 目標定位活動 {#targeting}

這些活動特定於定位。 它們可讓您定義對象，並使用交集、聯合或排除作業分割或結合這些對象，藉此建立一或多個目標對象。

* [建立對象](build-audience.md)：定義您的目標母體。 選取現有對象，或使用查詢建模器定義您自己的查詢。
* [變更資料來源](change-data-source.md)：變更工作流程工作表格的資料來源。
* [變更維度](change-dimension.md)：建立工作流程時變更目標維度。
* [合併](combine.md)：對傳入母體執行分段。 使用聯合、交集或排除。
* [重複資料刪除](deduplication.md)：移除傳入活動結果中的重複專案。
* [擴充](enrichment.md)：定義要在工作流程中處理的其他資料。 設定活動以使用其他資料完成輸出轉換。
* [增量查詢](incremental-query.md)：依排程查詢資料庫。 每次執行此活動時，都會排除先前執行的結果，僅鎖定新元素。
* [調解](reconciliation.md)：定義Adobe Campaign資料庫中的資料與工作表中的資料之間的連結，例如從外部檔案載入的資料。
* [儲存對象](save-audience.md)：更新現有的對象，或從工作流程中的母體運算上游建立新的對象。
* [分割](split.md)：將傳入母體分割為數個子集。

## 資料管理活動 {#data}

這些活動專門用於操控和豐富人口資料。

* [擷取檔案](extract-file.md)：將資料從Adobe Campaign匯出至其他系統，做為外部檔案。
* [載入檔案](load-file.md)：使用儲存在外部檔案中的設定檔和資料。
* [傳輸檔案](transfer-file.md)：接收或傳送檔案、測試檔案是否存在，或列出伺服器上的檔案。 使用的通訊協定可以是伺服器對伺服器通訊協定或 HTTP 通訊協定。
* [JavaScript程式碼](javascript-code.md)：在工作流程的內容中執行JavaScript程式碼片段。
* [訂閱服務](subscription-services.md)：在單一動作中，訂閱或取消訂閱服務中的多個設定檔。
* [更新資料](update-data.md)：對資料庫中的欄位執行大量更新。 數個選項可讓您個人化資料更新。

## 管道活動 {#channel}

Adobe Campaign Web可讓您跨多個管道自動執行行銷活動。 將管道活動結合到畫布中，以建立跨管道工作流程，這些工作流程會根據客戶行為來觸發動作。 有下列&#x200B;**頻道**&#x200B;活動可用：電子郵件、簡訊、Android和iOS推播通知。 [瞭解如何在工作流程的內容中設定傳遞](channels.md)。

## 流程控制活動 {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="結束活動"
>abstract="「**結束**」活動可讓您以圖形方式標記工作流程的終點。此活動並不會造成任何功能性影響，因此為選用。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="外部訊號"
>abstract="結束活動引數中外部訊號區段的預留位置。 僅適用於協調的行銷活動。 不要DELETE"

下列活動僅限於整理和執行工作流程。這些活動的主要任務是協調其他活動：

* [並加入](and-join.md)：同步處理工作流程的多個執行分支。
* **結束**：以圖形方式標示工作流程的結束。 此活動並不會造成任何功能性影響，因此為選用。
* [外部訊號](external-signal.md)：從其他工作流程或API呼叫觸發工作流程執行。
* [分支](fork.md)：建立出站轉變，以同時啟動多個活動。
* [排程器](scheduler.md)：在工作流程啟動時排程。
* [測試](test.md)：根據指定的條件啟用轉換。
* [等待](wait.md)：暫時暫停執行工作流程的一部分。