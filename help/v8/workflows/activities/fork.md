---
audience: end-user
title: 使用「分支」工作流程活動
description: 了解如何使用「分支」工作流程活動
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 97%

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

「**分支**」活動是一種&#x200B;**流程控制**&#x200B;活動。其可讓您建立出站轉變，以同時啟動多個活動。

## 設定分叉活動{#fork-configuration}

請按照以下步驟設定「**分支**」活動：

![](../assets/workflow-fork.png)

1. 在您的工作流程中新增一個「**分支**」活動。
1. 若要新增傳出轉變，請按一下「**新增轉變**」。預設情況下，會定義兩種轉變。
1. 對每種轉變新增標籤。

## 範例{#fork-example}

在下面的範例中，我們會使用兩種&#x200B;**分支**&#x200B;活動：

* 一個在兩個查詢之前，以同時執行查詢。
* 一個在交集之後，以同時傳送電子郵件和簡訊給目標母體。

![](../assets/workflow-fork-example.png)
