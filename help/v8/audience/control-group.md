---
audience: end-user
title: 設定控制組
description: 瞭解如何在Campaign網頁使用者介面中設定訊息的控制組
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 37%

---

# 設定控制組 {#control-group}

控制組是從傳送中排除的子族群。 您可以定義控制組以避免傳送訊息給部分對象，並將傳送後的行為與主要目標進行比較。 此選項可協助您測量行銷活動的影響。

➡️ [在影片中探索此功能](create-audience.md#video)

## 啟用控制組{#add-a-control-group}

若要新增控制組，請在定義傳送對象時啟用選項。 可以從主要目標隨機擷取控制組和/或從特定群體中選取。因此，定義控制組的主要方法有兩種：

* 從主要目標擷取輪廓。
* 從清單中排除某些設定檔，或根據查詢中定義的條件排除某些設定檔。

定義控制組時，您可以結合這兩種方法。

所有在傳遞準備步驟中屬於控制組的輪廓將會從主要目標中移除。他們並不會收到訊息。

>[!CAUTION]
>
>[從外部檔案](file-audience.md)載入目標群體時，您不能使用控制組。

若要新增控制組至傳遞，請從傳遞建立畫面的&#x200B;**對象**&#x200B;區段啟動&#x200B;**[!UICONTROL 啟用控制組]**&#x200B;切換按鈕。

![啟用控制組選項](assets/control-group1.png)


## 從目標中擷取 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="擷取模式"
>abstract="對照組是一組從傳遞排除的設定檔。若要定義控制組，您可以選擇從目標群體中隨機或基於排序、百分比或固定數量的輪廓中擷取。"


### 建立控制組 {#build-extract-target}

若要定義控制組，您可以選擇從目標人口中隨機或基於排序、百分比或固定數量的設定檔中擷取。 如果您偏好新增額外母體，請選擇&#x200B;**無擷取**&#x200B;選項，並選取額外母體[，詳情請參閱此處](#extra-population)。

首先，定義從目標中擷取設定檔的方式：隨機或根據排序。

在&#x200B;**控制群組**&#x200B;區段下，選擇&#x200B;**擷取模式**：

* **隨機**：在準備傳遞時，Adobe Campaign 將隨機擷取與百分比或您設定為大小限制的最大數量對應的多個輪廓。

* **按屬性排名**：此選項可讓您根據特定排序順序中的特定屬性排除一組輪廓。


然後使用&#x200B;**大小限制**&#x200B;區段來設定您需要從主要目標擷取的設定檔數目。 可以是原始數字（例如要排除的50個設定檔）或初始對象的百分比（例如主要目標的5%）。


### 控制組範例{#control-group-sample}

例如，若要建立具有100個最新設定檔的控制組，請遵循下列步驟：

1. 選取&#x200B;**年齡**&#x200B;欄位作為排序條件。 保留&#x200B;**遞增**&#x200B;排序選項。
1. 新增&#x200B;**建立日期**&#x200B;欄位。 變更為&#x200B;**遞減**&#x200B;排序選項。
1. 在&#x200B;**大小限制**&#x200B;區段中將100定義為臨界值。

   ![](assets/control-group2.png){zoomable="yes"}

然後從主要目標中排除這100個最年輕的設定檔。

### 檢查您的控制組 {#check-control-group}

您可以檢視記錄以檢查和識別排除的輪廓。讓我們以隨機排除五個輪廓為範例。

![](assets/control-group4.png){zoomable="yes"}

在準備傳送後，您可以檢閱套用排除專案的方式：

* 在傳送前，在傳遞儀表板中檢查&#x200B;**要排除** KPI。

  ![](assets/control-group5.png){zoomable="yes"}

* 在傳送記錄檔中， 「記錄檔」索引標籤會顯示排除步驟。

  ![](assets/control-group-sample-logs.png){zoomable="yes"}
<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}
-->

* **排除原因**&#x200B;索引標籤會顯示每個型別規則的排除設定檔數目。

  ![](assets/control-group7.png){zoomable="yes"}

如需傳遞記錄的詳細資訊，請參閱本[章節](../monitor/delivery-logs.md)。

## 新增額外群體 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="額外群體"
>abstract="對照組是一組從傳遞排除的設定檔。定義控制組的另一種方法是選取現有對象或定義查詢從傳遞對象中排除特定群體。"

定義控制組的另一種方式是選取現有對象中的特定母體，或藉由定義查詢來進行。

從&#x200B;**控制組**&#x200B;定義畫面的「**額外群體**」區段，按一下「**[!UICONTROL 選取客群]**」按鈕。

![](assets/control-group3.png){zoomable="yes"}

* 若要使用現有客群，按一下「**選取客群**」。若要了解詳細資訊，請參閱[本章節](add-audience.md)。

* 若要定義新的查詢，請選取&#x200B;**建立您自己的**，並使用查詢模型工具定義排除條件。 若要了解詳細資訊，請參閱[本章節](../query/query-modeler-overview.md)。

包含在對象中或符合查詢結果的設定檔是從傳遞目標中排除的&#x200B;**個**：它們沒有收到任何訊息。

## 比較結果{#control-group-results}

傳送後，您可以擷取傳送記錄檔，以比較未接收通訊的設定檔與有效目標之間的行為。 您也可以使用傳送記錄來建置新目標定位。

若要檢視已從目標移除的設定檔，請檢查&#x200B;**傳遞記錄**。 在本節](#check-control-group)瞭解更多[。
