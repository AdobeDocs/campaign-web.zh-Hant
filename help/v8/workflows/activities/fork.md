---
audience: end-user
title: 使用「分支」工作流程活動
description: 了解如何使用「分支」工作流程活動
badge: label="Alpha"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 91%

---


# 分支 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分支活動"
>abstract="「分支」活動可讓您建立傳出轉變，以同時啟動多個活動。"

## 設定

請按照以下步驟設定「**分支**」活動：

1. 在您的工作流程中新增一個「**分支**」活動。
1. 若要新增傳出轉變，請按一下「**新增轉變**」。預設情況下，會定義兩種轉變。
1. 對每種轉變新增標籤。

## 範例

在下列範例中，我們使用 **分支** 活動：

* 一個在兩個查詢之前，以同時執行查詢。
* 一個在交集之後，以同時傳送電子郵件和簡訊給目標母體。

![](../assets/workflow-fork-example.png)

