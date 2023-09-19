---
audience: end-user
title: 使用變更維度工作流程活動
description: 瞭解如何使用變更維度工作流程活動
badge: label="Beta"
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---


# 變更維度 {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="產生補充"
>abstract="您可以產生具有剩餘母體的其他出站轉變，該母體已排除為重複。 若要這麼做，請開啟 **產生補充** 選項"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="變更維度活動"
>abstract="此活動可讓您在建立對象時變更目標維度。 它會根據資料範本和輸入維度來移動軸。 例如，您可以從「合約」維度切換至「客戶」維度。"

此 **變更維度** 活動是 **目標定位** 活動。 此活動可讓您在建立對象時變更目標維度。 此活動會根據資料範本和輸入維度移動軸。 例如，您可以從「合約」維度切換至「客戶」維度。

## 設定變更維度活動 {#configure}

請依照下列步驟設定 **變更維度** 活動：

1. 新增 **變更維度** 活動至您的工作流程。

   ![](../assets/workflow-change-dimension.png)

1. 定義 **新增目標維度**. 在維度變更期間，會保留所有記錄。 尚未提供其他選項。

1. 執行工作流程以檢視結果。 比較變更維度活動前後表格中的資料，並比較工作流程表格的結構。

## 範例 {#example}


