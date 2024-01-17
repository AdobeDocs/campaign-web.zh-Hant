---
audience: end-user
title: 使用「組合」工作流程活動
description: 了解如何使用「組合」工作流程活動
badge: label="Beta"
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: 523a43bef4f179740a96039ac2fc5f4f858aa1dc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 84%

---

# 組合 {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="組合活動"
>abstract="「**組合**」活動可讓您對傳入族群執行分段。您因此可以組合好幾個族群、排除其中的一部分或僅保留幾個目標通用資料。"


此 **合併** 活動是 **目標定位** 活動。 此活動則可讓您對傳入母體執行分段。您因此可以組合好幾個母體、排除其中的一部分或僅保留幾個目標通用資料。以下是可用的分段類型：

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* 「**聯合**」可讓您將多個活動的結果重新分組至單一目標。
* 「**交集**」活動可讓您僅保留活動中不同傳入母體的通用元素。
* 「**排除**」可讓您根據特定條件從一個母體中排除元素。

## 設定合併活動 {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="交集合併選項"
>abstract="交集活動可讓您僅保留活動中不同傳入母體的通用元素。在「要加入的集合」一節中，勾選您之前希望加入的所有活動。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="排除合併選項"
>abstract="「排除」可讓您根據特定條件從一個母體中排除元素。在「要加入的集合」一節中，勾選您之前希望加入的所有活動。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="選取分段類型"
>abstract="選取組合對象的方式：聯合、交集或排除。"

請按照以下常見步驟開始設定「**組合**」活動：

![](../assets/workflow-combine.png)

1. 新增多個活動，例如「**建置對象**」活動，以形成至少兩個不同的執行分支。
1. 對上述的任一個分支新增「**組合**」活動。
1. 選取分段類型：[聯合](#union)、[交集](#intersection)或是[排除](#exclusion)。
1. 按一下&#x200B;**「繼續」**。
1. 在「**要加入的集合**」一節中，勾選您之前希望加入的所有活動。

## 聯合 {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="交集調和選項"
>abstract="選取調節類型，以定義處理重複項目的方式。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="調和選項"
>abstract="選取「**調和類型**」，以定義處理重複項目的方式。"

在 **合併** 活動，您可以設定 **聯集**. 為此，您需要選取 **調解型別** 若要定義重複專案的處理方式，請執行下列步驟：

* **僅限索引鍵**：這是預設模式。當來自不同入站轉變的元素具有相同索引鍵時，活動只會保留一個元素。如果入站母體是同質的，則只能使用此選項。
* **選取的欄**：選取此選項可定義套用資料協調的欄清單。 首先，必須選取主要集合 (其中包含來源資料)，然後指定用於加入的欄。

## 交集 {#combine-intersection}

在 **合併** 活動，您可以設定 **交集**. 為此，您需要遵循以下額外步驟：

1. 選取「**調節類型**」，以定義處理重複項目的方式。請參閱[聯合](#union)一節。
1. 如果您希望處理剩餘的母體，可勾選「**產生補充集**」選項。此補充集會包含所有傳入活動減去交集的聯合結果。然後，額外的傳出轉變會新增到活動中。

## 排除 {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="排除規則"
>abstract="如有必要，您可以操控傳入表格。事實上，若要從另一個維度排除目標，必須將此目標傳回主要目標的同一目標定位維度。為了進行此步驟，請按一下「排除規則」一節中的「新增規則」，並指定維度變更條件。資料調節會透過屬性或加入執行。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="選取要組合的集合"
>abstract="在「**要加入的集合**」一節中，從傳入轉變中選取「**主要集合**」。這是從中排除元素的集。其他集會先設定相符的元素，然後才會從主要集予以排除。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="排除規則"
>abstract="如有必要，您可以操控傳入表格。事實上，若要從另一個維度排除目標，必須將此目標傳回主要目標的同一目標定位維度。為了進行此步驟，請按一下「排除規則」一節中的「新增規則」，並指定維度變更條件。資料調節會透過屬性或加入執行。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="合併產生補充集"
>abstract="開啟「產生補充」選項，在其他轉變中處理剩餘母體。"

在 **合併** 活動，您可以設定 **排除**. 為此，您需要遵循以下額外步驟：

1. 在「**要加入的集合**」一節中，從傳入轉變中選取「**主要集合**」。這是從中排除元素的集。其他集會先設定相符的元素，然後才會從主要集予以排除。
1. 如有必要，您可以操控傳入表格。事實上，若要從另一個維度排除目標，必須將此目標傳回主要目標的同一目標定位維度。為了進行此步驟，請按一下「**排除規則**」一節中的「**新增規則**」，並指定維度變更條件。資料調節會透過屬性或加入執行。
1. 如果您希望處理剩餘的母體，可勾選「**產生補充集**」選項。請參閱[交集](#intersection)一節。

## 範例{#combine-examples}

在以下範例中，我們使用 **合併** 活動，然後我們新增 **聯合** 擷取兩個查詢的所有設定檔：18至27歲的人和34至40歲的人。

![](../assets/workflow-union-example.png)

以下範例會顯示兩個查詢活動之間的&#x200B;**交集**。在這裡會將它用於擷取年齡在 18 至 27 歲之間且已提供其電子郵件地址的設定檔。

![](../assets/workflow-intersection-example.png)

以下「**排除**」範例會顯示兩個查詢，設定為篩選年齡在 18 歲至 27 歲之間且擁有 Adob&#x200B;&#x200B;e 電子郵件網域的設定檔。然後從第一個集合中排除包含 Adobe 電子郵件地址網域的設定檔。

![](../assets/workflow-exclusion-example.png)
