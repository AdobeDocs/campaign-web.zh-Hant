---
audience: end-user
title: 使用「分支」工作流程活動
description: 了解如何使用「分支」工作流程活動
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 55%

---


# 分支 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="分支活動"
>abstract="**分支**&#x200B;活動可讓您建立傳出轉變，以同時啟動多個活動。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分支活動轉變"
>abstract="依預設，透過&#x200B;**分支**&#x200B;活動建立二個轉變。按一下&#x200B;**新增轉變**&#x200B;按鈕以定義額外的傳出轉變，並輸入其標籤。"

「**分支**」活動是一種&#x200B;**流程控制**&#x200B;活動。它可讓您建立出站轉變，以同時啟動多個活動。

## 設定分叉活動 {#fork-configuration}

請按照以下步驟設定「**分支**」活動：

![工作流程分叉活動設定熒幕擷圖](../assets/workflow-fork.png)

1. 在您的工作流程中新增一個「**分支**」活動。
1. 若要新增傳出轉變，請按一下「**新增轉變**」。依預設，會定義兩個轉接。
1. 為每個轉變新增標籤。

## 範例 {#fork-example}

在下列範例中，使用了兩個&#x200B;**Fork**&#x200B;活動：

* 兩個查詢前一個，以同時執行它們。
* 在交叉點後一個，同時傳送電子郵件和簡訊給目標母體。

![工作流程分叉範例熒幕擷圖](../assets/workflow-fork-example.png)
