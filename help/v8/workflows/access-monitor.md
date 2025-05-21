---
audience: end-user
title: 使用 Adobe Campaign Web 建立工作流程
description: 了解如何使用 Adobe Campaign Web 建置工作流程
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 17%

---

# 存取並管理工作流程 {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="工作流程"
>abstract="在此畫面中，您可以存取獨立和行銷活動工作流程的完整清單、檢查其目前狀態、上次/下次執行日期並建立新的工作流程。瀏覽到「範本」分頁以存取可用的工作流程範本。"

**[!UICONTROL 工作流程]**&#x200B;功能表提供工作流程完整清單的存取權。 此清單包含從此畫面建立的&#x200B;**獨立工作流程**，以及在行銷活動中建立的&#x200B;**行銷活動工作流程**。

![顯示獨立工作流程和行銷活動工作流程的工作流程清單畫面](assets/workflow-list.png){zoomable="yes"}

清單中的每個工作流程都會顯示其目前[狀態](#status)、上次執行或修改的時間，以及下一個排程執行日期和時間的相關資訊。

按一下位於清單右上角的自訂配置&#x200B;]**圖示的**[!UICONTROL &#x200B;設定欄，以自訂顯示的欄。 這可讓您新增其他資訊至清單，例如每個工作流程的最後一個錯誤活動或套用的目標維度。

此外，搜尋列和篩選器也可用於簡化清單內的搜尋。 例如，篩選工作流程以僅顯示屬於某個行銷活動的行銷活動或是在特定日期範圍內處理的行銷活動。

若要複製或刪除工作流程，請按一下省略符號按鈕，然後選取&#x200B;**[!UICONTROL 複製]**&#x200B;或&#x200B;**[!UICONTROL 刪除]**。

>[!NOTE]
>
>您可以複製進行中的工作流程，但無法刪除它。

## 工作流程的狀態 {#status}

工作流程可以有多個狀態：

* **[!UICONTROL 草稿]**：工作流程已建立並儲存。
* **[!UICONTROL 進行中]**：工作流程目前正在執行。
* **[!UICONTROL 已完成]**：工作流程執行完成。
* **[!UICONTROL 已暫停]**：工作流程已暫停。
* **[!UICONTROL 錯誤]**：工作流程發生錯誤。 開啟工作流程並存取記錄檔和任務，以識別錯誤並加以解決。 [瞭解如何監視記錄檔和工作](start-monitor-workflows.md#logs-tasks)

有關如何啟動及監視工作流程執行的詳細資訊，請參閱[此頁面](start-monitor-workflows.md)。

## 工作流程範本 {#templates}

**[!UICONTROL 範本]**&#x200B;索引標籤會列出所有可用的工作流程範本。

工作流程範本包含預先設定的活動和整體屬性設定，可重複用於建立新工作流程。

從現有工作流程或從頭開始建立工作流程範本。 [瞭解如何建立工作流程範本](create-workflow.md#workflow-templates)