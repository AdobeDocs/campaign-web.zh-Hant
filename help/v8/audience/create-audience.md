---
audience: end-user
title: 建立對象
description: 瞭解如何在Adobe Campaign Web中建立對象
badge: label="Beta"
source-git-commit: 1b17dcbdaadcbf45b2c26d9099e6d139143d253c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 1%

---


# 建立對象 {#create-audiences}

Campaign Web可讓您建立工作流程，將現有對象合併到視覺畫布中。 透過合併各種工作流程活動（例如分割或排除），您可以產生新的和完善的對象。

當您完成工作流程後，產生的對象會自動與您現有的對象一起儲存在Campaign網頁中。 然後便可在行銷活動或獨立傳送中鎖定這些對象。

若要建立對象，請遵循下列步驟：

1. 導覽至 **[!UICONTROL 受眾]** 功能表，然後按一下 **[!UICONTROL 建立對象]** 按鈕的位置。
1. 為對象提供標籤。
1. 展開 **[!UICONTROL 其他選項]** 區段來設定進階對象引數。

   依預設，對象會建立到 **[!UICONTROL 設定檔和目標]** / **[!UICONTROL 清單]** explorer功能表。 您可以使用變更預設儲存位置 **[!UICONTROL 資料夾]** 欄位。

   ![](assets/audiences-settings.png)

1. 設定對象設定後，請按一下 **[!UICONTROL 建立對象]** 按鈕。

1. 工作流程畫布隨即顯示，其中包含兩個預設活動：

   * **[!UICONTROL 建立對象]**：這是工作流程的起點，可讓您建立受眾，並將其用作工作流程的基礎。
   * **[!UICONTROL 儲存對象]**：這代表工作流程的最後一步，可讓您將結果儲存為新對象。

1. 視需要新增任意數量的活動，以自訂您的工作流程。 有關如何設定工作流程活動的詳細資訊，請參閱 [工作流程檔案](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >管道活動不適用於對象工作流程。

   ![](assets/audience-creation-canvas.png)

1. 當工作流程準備就緒時，按一下 **[!UICONTROL 開始]** 以執行。

1. 工作流程會儲存在 **[!UICONTROL 工作流程]** 清單，而可在中存取產生的對象 **[!UICONTROL 受眾]** 清單。 [瞭解如何監視和管理對象](access-audiences.md)
