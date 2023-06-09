---
audience: end-user
title: 使用取用工作流程活動
description: 瞭解如何使用復本工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: 1ac80ffaabea210bbc02588475ad6e81af4820b1
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 21%

---


# 分支 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分叉活動"
>abstract="「分支」活動可讓您建立出站轉變，以同時啟動多個活動。"

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

