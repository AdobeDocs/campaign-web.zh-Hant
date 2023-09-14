---
audience: end-user
title: 建立對象
description: 瞭解如何在Adobe Campaign Web中建立對象
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 1%

---


# 建立對象 {#create-audiences}

Campaign Web可讓您建立工作流程，其中您可以將現有對象合併到視覺畫布中，並利用各種活動（分割、排除……）來建立新對象。

完成後，產生的受眾會連同現有受眾一併儲存至Campaign Web中，並可在獨立傳遞或行銷活動中運用以鎖定個人。

## 建立您的第一個對象 {#create}

若要建立對象，請遵循下列步驟：

1. 導覽至 **[!UICONTROL 受眾]** 功能表並按一下 **[!UICONTROL 建立對象]** 按鈕。
1. 為對象提供標籤。
1. 展開其他選項區段，設定對象的進階器引數。

   >[!NOTE]
   >
   >依預設，會在「設定檔和目標/清單探索者」選單中建立對象。 您可以變更中的預設儲存位置 **[!UICONTROL 資料夾]** 欄位。

1. 設定對象設定後，按一下 **[!UICONTROL 建立對象]** 按鈕。

1. 工作流程畫布隨即顯示，其中包含兩個預設活動：

   * **[!UICONTROL 建立對象]**：工作流程的起點。 此活動可讓您選取一或多個對象作為工作流程的基礎。
   * **[!UICONTROL 儲存對象]**：工作流程的最後一步。 此活動可讓您將工作流程的結果儲存至新受眾。

1. 視需要新增儘可能多的活動以設定工作流程。 有關如何設定各種活動的詳細資訊，請參閱 [工作流程檔案](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >管道活動不適用於對象工作流程。

   ![](assets/audience-creation-canvas.png)

1. 當工作流程準備就緒時，按一下 **[!UICONTROL 開始]** 以執行。

1. 工作流程會儲存至 **[!UICONTROL 工作流程]** 清單以及產生的對象移入 **[!UICONTROL 受眾]** 清單。 [瞭解如何監視和管理對象](access-audiences.md)
