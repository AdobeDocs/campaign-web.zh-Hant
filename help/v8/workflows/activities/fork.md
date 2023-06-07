---
audience: end-user
title: 使用取用工作流程活動
description: 瞭解如何使用復本工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# 分支 {#fork}

此 **分支** 活動是 **流量控制** 活動。 它可讓您建立出站轉變，以同時開始多個活動。

## 設定

請依照下列步驟設定 **分支** 活動：

1. 新增 **分支** 活動至您的工作流程。
1. 按一下 **新增轉變** 以新增出站轉變。 依預設，會定義兩個轉接。
1. 為每個轉變新增標籤。

## 範例

以下範例中，我們使用2個 **分支** 活動：

* 兩個查詢前一個，以便同時執行。
* 在交叉點後一個，同時傳送電子郵件和簡訊給目標母體。

![](../assets/workflow-fork-example.png)

