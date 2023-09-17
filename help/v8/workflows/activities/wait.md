---
audience: end-user
title: 使用等待工作流程活動
description: 了解如何使用等待工作流程活動
badge: label="Beta"
source-git-commit: 173141ec198b4d451a7b388f0e28a29230a11396
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 91%

---


# 等待 {#wait}


>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="等待活動"
>abstract="此 **等待** 活動用於延遲從活動到另一個活動的轉變。"


「**等待**」活動是一種&#x200B;**流程控制**&#x200B;活動。此活動用於允許正在執行的兩個活動之間經過一定的時間。例如，若要在電子郵件傳送活動後等候數天，請先分析此期間產生的開啟次數和點按次數，再執行任何後續操作 (提醒電子郵件、建立對象等)。

## 設定

請按照以下步驟設定&#x200B;**等待**&#x200B;活動：

1. 在您的工作流程中新增一個&#x200B;**等待**&#x200B;活動。

1. 指定傳入和傳出轉變之間等待的&#x200B;**持續時間**。

1. 在&#x200B;**期間**&#x200B;欄位中選取時間單位：秒、分鐘、小時。

## 範例

以下範例會說明典型使用案例中的 **等待**&#x200B;活動。已傳送活動的電子郵件邀請。傳送後 24 小時，會將簡訊傳送給同一個母體。

![](../assets/workflow-wait-example.png)
