---
audience: end-user
title: 使用變更維度工作流程活動
description: 瞭解如何使用變更維度工作流程活動
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: 52b129be88e48dd70c0f55b404fd3bbe699dbebb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 26%

---

# 變更維度 {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="產生補充集"
>abstract="您可以使用剩餘族群 (其已因重複而排除) 產生額外的出站轉變。若要這樣做，請開啟「**產生補充集**」選項"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="變更維度活動"
>abstract="此活動可讓您在建立對象時變更目標定位維度。其會根據資料範本和輸入維度來移動軸。例如，您可以從「合約」維度切換到「客戶」維度。"

此 **變更維度** 活動是 **目標定位** 活動。 此活動可讓您在建立工作流程時變更目標維度。 其會根據資料範本和輸入維度來移動軸。[進一步瞭解目標維度](../../audience/about-recipients.md#targeting-dimensions)

例如，您可以將工作流程的目標維度從「收件者」切換至「訂閱者應用程式」，以傳送推播通知給目標收件者。

>[!IMPORTANT]
>
>請注意 **[!UICONTROL 變更維度]** 和 **[!UICONTROL 變更資料來源]** 活動不應新增為一列。 如果您需要連續使用兩個活動，請務必加入 **[!UICONTROL 擴充]** 兩者之間的活動。 這可確保正確執行並防止潛在的衝突或錯誤。

## 設定變更維度活動 {#configure}

請依照下列步驟設定 **變更維度** 活動：

1. 新增 **變更維度** 活動至您的工作流程。

   ![](../assets/workflow-change-dimension.png)

1. 定義 **新增目標維度**. 在維度變更期間，會保留所有記錄。 尚未提供其他選項。

1. 執行工作流程以檢視結果。 比較變更維度活動前後表格中的資料，並比較工作流程表格的結構。

## 範例 {#example}

在此範例中，我們要傳送SMS傳送給已購買的所有設定檔。 為此，我們先使用 **[!UICONTROL 建立對象]** 連結至自訂「購買」目標維度的活動，以定位發生的所有購買。

然後我們使用 **[!UICONTROL 變更維度]** 活動以將工作流程目標維度切換為「收件者」。 這可讓我們鎖定符合查詢的收件者。

![](../assets/workflow-change-dimension-example.png)
