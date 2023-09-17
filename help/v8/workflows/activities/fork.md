---
audience: end-user
title: 使用「分支」工作流程活動
description: 了解如何使用「分支」工作流程活動
badge: label="Beta"
source-git-commit: 173141ec198b4d451a7b388f0e28a29230a11396
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 68%

---


# 分支 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="分支活動"
>abstract="**分支**&#x200B;活動可讓您建立傳出轉變，以同時啟動多個活動。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="建立活動轉變分支"
>abstract="依預設，會使用建立兩個轉變 **分支** 活動。 按一下 **新增轉變** 按鈕以定義其他出站轉變，並輸入其標籤。"

此 **分支** 活動是 **流量控制** 活動。 它可讓您建立出站轉變，以同時啟動多個活動。

## 設定

請按照以下步驟設定「**分支**」活動：

1. 在您的工作流程中新增一個「**分支**」活動。
1. 若要新增傳出轉變，請按一下「**新增轉變**」。預設情況下，會定義兩種轉變。
1. 對每種轉變新增標籤。

## 範例

在下面的範例中，我們會使用兩種&#x200B;**分支**&#x200B;活動：

* 一個在兩個查詢之前，以同時執行查詢。
* 一個在交集之後，以同時傳送電子郵件和簡訊給目標母體。

![](../assets/workflow-fork-example.png)

