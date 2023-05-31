---
audience: end-user
title: 使用建立對象工作流程活動
description: 瞭解如何使用建立對象工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 16%

---


# 建置對象 {#build-audience}

此活動可讓您定義對象。 您可以選取現有的Campaign對象，或使用規則產生器來定義自己的查詢。

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

請依照下列步驟設定 **建立對象** 活動：

1. 新增「建置」對象活動。
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
