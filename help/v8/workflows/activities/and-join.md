---
audience: end-user
title: 使用「合併連結」工作流程活動
description: 了解如何使用「合併連結」工作流程活動
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 99%

---

# 合併連結 {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join 活動"
>abstract="**合併連結**&#x200B;活動可讓您同步處理工作流程的多個執行分支。一旦所有前面的活動完成，就會觸發此活動。這讓您可以在確保特定活動已完成後再繼續執行工作流程。"

「**合併連結**」活動是一種&#x200B;**流程控制**&#x200B;活動。此活動可讓您同步處理工作流程的多個執行分支。

此活動只會在所有傳入轉變啟動後，才會觸發其傳出轉變，換句話說，會在所有之前的活動完成後觸發。這讓您可以在確保特定活動已完成後再繼續執行工作流程。

## 設定 And-join 活動{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="設定 AND-join 活動"
>abstract="選取您要參加的活動。在「**主要集合**」下拉選單中，選擇您要保留的傳入轉變族群。"

請按照以下步驟設定「**合併連結**」活動：

![](../assets/workflow-andjoin.png)

1. 新增多個活動，例如「管道」活動，以形成至少兩個不同的執行分支。
1. 新增「**合併連結**」活動至任何分支。
1. 在「**合併選項**」一節中，勾選您之前希望加入的所有活動。
1. 在「**主要集合**」下拉選單中，選擇您要保留的傳入轉變母體。傳出轉變只能包含其中一個傳入轉變母體。

## 範例{#and-join-example}

以下範例顯示兩個工作流程分支，各包含電子郵件和簡訊傳遞。同時啟用兩個傳入轉變時，「合併連結」即會觸發。只有在兩個傳遞都完成後，接著才會傳送推播通知。

![](../assets/workflow-andjoin-example.png){zoomable=&quot;yes&quot;}
