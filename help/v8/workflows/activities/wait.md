---
audience: end-user
title: 使用等待工作流程活動
description: 瞭解如何使用等待工作流程活動
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 29%

---


# 等待 {#wait}

此 **等待** 活動是 **流量控制** 活動。 它可用來讓兩個執行之活動之間有特定時間間隔。 例如，若要在電子郵件傳送活動後等候數天，請先分析此期間產生的開啟次數和點按次數，再執行任何後續操作（提醒電子郵件、建立閱聽眾等）。

## 設定

請依照下列步驟設定 **等待** 活動：

1. 新增 **等待** 活動放入您的工作流程。

1. 指定 **持續時間** 入站和出站轉變之間的等待時間。

1. 選取時間單位 **週期** 欄位：秒、分、小時。

## 範例

下列範例說明 **等待** 活動。 已傳送活動的電子郵件邀請。SMS傳送會在傳送24小時後傳送給相同母體。

![](../assets/workflow-wait-example.png)
