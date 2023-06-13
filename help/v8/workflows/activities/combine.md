---
audience: end-user
title: 使用合併工作流程活動
description: 瞭解如何使用合併工作流程活動
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 11%

---


# 組合 {#combine}

此活動可讓您對入站母體執行分段。 因此，您可以合併多個母體、排除部分母體，或僅保留多個目標通用的資料。 可用的區段型別如下：

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* 此 **聯集** 可讓您將多個活動的結果重新分組為單一目標。
* 此 **交集** 可讓您僅保留活動中不同入站母體的共同元素。
* 此 **排除** 可讓您根據特定條件從一個母體中排除元素。

## 一般設定 {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="交集合併選項"
>abstract="交集可讓您僅保留活動中不同入站母體的共同元素。 在「要加入的集合」區段中，勾選所有先前要加入的活動。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="排除合併選項"
>abstract="排除可讓您根據特定條件從一個母體中排除元素。 在「要加入的集合」區段中，勾選所有先前要加入的活動。"

請依照下列常見步驟開始設定 **合併** 活動：

1. 新增多個活動，例如 **建立對象** 至少形成兩個不同執行分支的活動。
1. 新增 **合併** 活動到任何先前的分支。
1. 選取分段型別： [聯合](#union)， [交集](#intersection) 或 [排除](#exclusion).
1. 按一下 **繼續**.
1. 在 **要聯結的集合** 區段，勾選所有您欲加入的先前活動。

## 聯合 {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="交集 調解選項"
>abstract="選取調解型別以定義如何處理重複專案。"

對於 **聯集**，您必須選取 **調解型別** 若要定義如何處理重複專案，請執行下列動作：

* **僅限金鑰**：這是預設模式。 當來自不同入站轉變的元素具有相同索引鍵時，活動只會保留一個元素。如果入站母體是同質的，則只能使用此選項。
* **選取的欄**：選取此選項可定義將套用資料協調的欄清單。 首先，必須選取主集（其中包含來源資料），然後指定用於加入的欄。

## 交集 {#intersection}

對於 **交集**，您需要依照以下額外步驟操作：

1. 選取 **調解型別** 以定義如何處理重複專案。 請參閱 [聯集](#union) 區段。
1. 您可以檢查 **產生補充** 選項（如果要處理剩餘母體）。 補碼將包含所有入站活動結果減去交集的聯合。 然後，會將額外的出站轉變新增至活動。

## 排除 {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="排除規則"
>abstract="必要時，您可以操作傳入表格。 事實上，若要從其他維度排除目標，此目標必須傳回至與主要目標相同的目標維度。 若要這麼做，請按一下「排除規則」區段中的「新增規則」 ，並指定維度變更條件。 資料調解可透過屬性或聯結來執行。"

對於 **排除**，您需要依照以下額外步驟操作：

1. 在 **要聯結的集合** 區段，選取 **主要集** 來自入站轉變。 這是從中排除元素的集。其他集會先設定相符的元素，然後才會從主要集予以排除。
1. 必要時，您可以操作傳入表格。 事實上，若要從其他維度排除目標，此目標必須傳回至與主要目標相同的目標維度。 若要這麼做，請按一下 **新增規則** 在 **排除規則** 並指定尺寸變更條件。 資料調解可透過屬性或聯結來執行。
1. 您可以檢查 **產生補充** 選項（如果要處理剩餘母體）。 請參閱 [交集](#intersection) 區段。

## 範例

在以下範例中，我們新增了 **聯合** 這會擷取這兩個查詢的所有設定檔：18至27歲的人和34至40歲的人。

![](../assets/workflow-union-example.png)

下列範例顯示 **交集** 介於兩個查詢活動之間。 此處用於擷取18至27歲之間且已提供其電子郵件地址的設定檔。

![](../assets/workflow-intersection-example.png)

下列專案 **排除** 範例顯示兩個查詢，其設定為篩選年齡介於18到27歲之間且具有Adobe電子郵件網域的設定檔。 之後，會從第一個集合中排除具有Adobe電子郵件網域的設定檔。

![](../assets/workflow-exclusion-example.png)


