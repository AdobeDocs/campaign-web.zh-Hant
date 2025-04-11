---
audience: end-user
title: 使用等待工作流程活動
description: 了解如何使用等待工作流程活動
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 39%

---

# 等待 {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="等待活動"
>abstract="**等待**&#x200B;活動用於延遲從一個活動到另一個活動的轉換。"

「**等待**」活動是一種&#x200B;**流程控制**&#x200B;活動。它允許在執行兩個活動之間傳遞的特定時間。 例如，它可用於在電子郵件傳送活動後等候數天，然後分析在此期間產生的開啟次數和點按次數，再執行後續操作，例如傳送提醒電子郵件或建立對象。

## 設定 {#wait-configuration}

請按照以下步驟設定&#x200B;**等待**&#x200B;活動：

1. 在您的工作流程中新增一個&#x200B;**等待**&#x200B;活動。

1. 指定傳入和傳出轉變之間等待的&#x200B;**持續時間**。

1. 在&#x200B;**期間**&#x200B;欄位中選取時間單位：秒、分鐘、小時或天。

## 範例 {#wait-example}

以下範例會說明典型使用案例中的 **等待**&#x200B;活動。已傳送活動的電子郵件邀請。24小時後，會傳送SMS傳送給相同母體。

![使用等待活動在電子郵件邀請後24小時傳送SMS的工作流程範例。](../assets/workflow-wait-example.png)