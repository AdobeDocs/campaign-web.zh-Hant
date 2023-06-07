---
audience: end-user
title: 使用建立對象工作流程活動
description: 瞭解如何使用建立對象工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 11%

---


# 建置對象 {#build-audience}

此 **建立對象** 活動是 **目標定位** 活動。 此活動可讓您定義將進入工作流程的對象。 在行銷活動工作流程的內容中傳送訊息時，訊息對象不會定義在管道活動中，而是定義在 **建立對象** 活動。

若要定義對象母體，您可以：

* 選取在使用者端主控台中建立為清單的現有對象。
* 選取Adobe Experience Platform對象。
* 定義並結合篩選條件，以使用規則產生器建立新對象。

>[!NOTE]
>
>在此內容中，您無法從檔案載入對象。 為此，您需要建立獨立傳送。 [了解更多](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 設定

請依照下列步驟設定 **建立對象** 活動：

1. 新增 **建立對象** 活動。
1. 定義標籤。
1. 定義對象型別： **建立您自己的** 或 **讀取對象**.

若要建立自己的查詢，請遵循下列額外步驟：

1. 選取 **建立您自己的（查詢）**.
1. 選擇 **目標維度**. 目標定位維度可讓您定義作業的目標母體：收件者、合約受益人、操作者、訂閱者等。依預設，會從收件者中選取目標。 請參閱 [v8檔案](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. 按一下 **繼續**.
1. 使用規則產生器來定義您的查詢，就像在設計新電子郵件時建立對象一樣。 請參閱本[章節](../../audience/segment-builder.md)。

若要選取現有對象，請遵循下列步驟：

1. 選取 **讀取對象**.
1. 按一下 **繼續**.
1. 選取您的對象，就像在設計新電子郵件時使用對象一樣。 請參閱本[章節](../../audience/add-audience.md)。

## 範例

以下是包含兩個的工作流程範例 **建立對象** 活動。 第一個目標是撲克玩家受眾，然後是電子郵件傳送。 第二個是以VIP使用者端對象為目標，然後是SMS傳送。

![](../assets/workflow-audience-example.png)