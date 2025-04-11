---
title: Campaign Web 使用者介面工作流程的護欄和限制
description: 在 Campaign Web 使用者介面中使用工作流程時的護欄和限制
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 56%

---

# 工作流程的護欄和限制 {#guardrails-limitations}

當在 Campaign Web 使用者介面使用在 Campaign 用戶端主控台建立或修改的工作流程時，便會套用下方所列的護欄和限制。

請注意，儘管本頁面會針對在主控台與網路使用者介面使用工作流程說明主要考量，但並未涵蓋兩個介面之間的所有潛在不相容性。

## 工作流程活動 {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="活動不可編輯"
>abstract="當在主控台利用其他資料設定&#x200B;**查詢**&#x200B;或&#x200B;**擴充**&#x200B;活動時，Campaign Web 會將擴充資料納入考量，並傳遞至出站轉變，但無法編輯。"

Campaign Web 中尚不支援的工作流程活動為唯讀，並會顯示為不相容的活動。您仍然可以執行工作流程、傳送訊息、檢查記錄檔以及執行其他工作。 Campaign Web 使用者介面和 Campaign 用戶端主控台都可用的工作流程活動均可編輯。

| 主控台 | Web |
| --- | --- |
| ![熒幕擷圖顯示主控台中活動的限制](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![顯示網頁介面活動限制的熒幕擷圖](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

當在主控台利用其他資料設定&#x200B;**查詢**&#x200B;或&#x200B;**擴充**&#x200B;活動時，Campaign Web 會將擴充資料納入考量，並傳遞至出站轉變，但無法編輯。

| 主控台 | Web |
| --- | --- |
| ![顯示主控台中選項限制的熒幕擷圖](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![顯示網頁介面中選項限制的熒幕擷圖](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

在主控台中，「**擴充**」活動可以執行調和和擴充。如果您已在使用者端主控台的&#x200B;**擴充**&#x200B;活動中定義調解設定，則會在Campaign Web使用者介面中顯示為&#x200B;**調解**&#x200B;活動。

| 主控台 | Web |
| --- | --- |
| ![熒幕擷圖顯示主控台中的擴充活動](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![在網頁介面中顯示擴充活動的熒幕擷圖](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## 工作流程畫布 {#wkf-canvas}

在 Campaign Web 使用者介面建立新工作流程時，畫布僅支援單一進入點。不過，如果您在主控台中建立了具有多個進入點的工作流程，您可以在Campaign Web使用者介面中開啟及編輯該工作流程。

| 主控台 | Web |
| --- | --- |
| ![在主控台中顯示多個進入點的熒幕擷圖](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![在網頁介面中顯示多個進入點的熒幕擷圖](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

每次新增或移除活動時，節點的位置都會重新整理。 如果您在主控台中建立工作流程、使用Campaign Web使用者介面修改它，並在主控台中重新開啟它，您可能會注意到一些細微的定位不完美。 這對工作流程的流程和任務沒有影響。

| 初始工作流程 | 定位變更 |
| --- | --- |
| ![顯示初始工作流程定位的熒幕擷圖](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![熒幕擷圖顯示修改後的定位變更](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |