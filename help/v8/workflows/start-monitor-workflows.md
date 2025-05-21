---
audience: end-user
title: 使用 Adobe Campaign Web 建立工作流程
description: 了解如何使用 Adobe Campaign Web 建置工作流程
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 5%

---

# 開始並監控工作流程 {#start-monitor}

建立工作流程並設計要在畫布中執行的任務後，您就可以啟動它並監視其執行方式。

## 開始工作流程 {#start}

若要啟動工作流程，請導覽至&#x200B;**[!UICONTROL 工作流程]**&#x200B;功能表或相關的行銷活動，然後按一下畫布右上角的&#x200B;**[!UICONTROL 開始]**&#x200B;按鈕。

工作流程執行後，畫布中的每個活動都會依序執行，直到工作流程結束為止。

您可以使用視覺流量即時追蹤目標設定檔的進度。 這可讓您快速識別每個活動的狀態，以及活動中轉換的個人檔案數。

![正在進行工作流程執行的視覺化表示。](assets/workflow-execution.png){zoomable="yes"}

## 工作流程轉換 {#transitions}

在工作流程中，透過轉變從一個活動傳輸到另一個活動的資料會儲存在臨時工作表中。 此資料可針對每個轉變顯示。 若要顯示資料，請選取轉變以在熒幕右側開啟其屬性。

* 按一下&#x200B;**[!UICONTROL 預覽結構描述]**&#x200B;以顯示工作表的結構描述。
* 按一下&#x200B;**[!UICONTROL 預覽結果]**&#x200B;以檢視所選轉變中傳輸的資料。

![轉換屬性和資料預覽範例。](assets/transition.png){zoomable="yes"}

## 監視活動執行 {#activities}

每個活動方塊右上角的視覺指示器可讓您檢查其執行狀態：

| 視覺指示器 | 說明 |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | 活動目前正在執行。 |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | 活動需要您注意。 這可能涉及確認傳遞的傳送或採取必要行動。 |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | 活動發生錯誤。 若要解決此問題，請開啟工作流程記錄檔以取得詳細資訊。 |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | 已成功執行活動。 |

## 監視記錄和任務 {#logs-tasks}

監視工作流程記錄和任務是分析工作流程並確保其正常執行的關鍵步驟。 可從動作工具列和每個活動的屬性窗格中的&#x200B;**[!UICONTROL 記錄檔]**&#x200B;圖示存取記錄檔和工作。

**[!UICONTROL 記錄檔及工作]**&#x200B;功能表提供工作流程執行的歷史記錄，記錄所有使用者動作及遇到的錯誤。 此歷史記錄會儲存至工作流程[執行選項](workflow-settings.md)中指定的期間。 在此期間，會儲存所有訊息，即使在工作流程重新啟動後亦然。 如果您不想儲存先前執行的訊息，請按一下&#x200B;**[!UICONTROL 清除歷史記錄]**&#x200B;按鈕。

![工作流程記錄檔與工作介面的範例。](assets/workflow-logs.png){zoomable="yes"}

提供兩種資訊：

* **[!UICONTROL Log]**&#x200B;索引標籤包含所有工作流程活動的執行歷程記錄。 其會按時間順序，對執行的操作和執行錯誤進行索引。
* **[!UICONTROL 任務]**&#x200B;索引標籤詳細說明活動的執行順序。

在這兩個標籤中，您可以選擇顯示的欄及其順序、套用篩選器，並使用搜尋欄位來快速尋找所需的資訊。

## 工作流程執行命令 {#execution-commands}

右上角的動作列提供管理工作流程執行的命令。 您可以：

* **[!UICONTROL 開始]** / **[!UICONTROL 繼續]**&#x200B;工作流程的執行。 如果工作流程已暫停，則會繼續。 否則，它會啟動，並啟動初始活動。
* **[!UICONTROL 暫停]**&#x200B;工作流程的執行。 工作流程接著會採取暫停狀態。 在繼續之前，不會啟用任何新活動，但不會暫停進行中的作業。
* **[!UICONTROL 停止]**&#x200B;正在執行的工作流程。 然後，工作流程會採取已完成狀態。 如果可能的話，進行中的作業會中斷。 您無法從工作流程停止的位置繼續該工作流程。