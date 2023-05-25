---
audience: end-user
title: 設定控制組
description: 了解如何在 Campaign Web UI 中為您的訊息設定控制組
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Alpha" type="Positive"
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 97%

---

# 設定控制組 {#control-group}

您可以使用控制組來避免傳送訊息給部分觀眾，以評估行銷活動的影響。

為此，請在定義傳遞對象時，建立控制組。設定檔會隨機新增至控制組、篩選或不篩選，或根據標準。然後，您可以將接收到訊息之目標母體的行為與未作為目標之聯絡人的行為進行比較。

可以從主要目標隨機擷取控制組和/或從特定母體中選取。因此，定義控制組的主要方法有兩種：

* 從主要目標擷取設定檔。
* 根據查詢中定義的條件排除一些設定檔。

定義控制組時，可以使用這兩種方法。

所有在傳遞準備步驟中屬於控制組的設定檔將會從主要目標中移除。他們並不會收到訊息。

若要建立控制組，請在傳遞建立助理的「**對象**」區段中，按一下「**[!UICONTROL 設定控制組]**」按鈕。

![](assets/control-group1.png)

>[!CAUTION]
>
>載入目標母體時，無法使用控制組 [從外部檔案](file-audience.md).


## 從目標中擷取 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="從目標中擷取"
>abstract="若要定義控制組，您可以選擇從目標母體中隨機或基於排序、百分比或固定數量的設定檔中擷取。"

若要定義控制組，您可以選擇從目標母體中隨機或基於排序、百分比或固定數量的設定檔中擷取。

首先，定義從目標中擷取設定檔的方式：隨機或根據排序。

在「**從目標中擷取**」區段中，選擇一個&#x200B;**排除類型**：

* **隨機**：在準備傳遞時，Adobe Campaign 將隨機擷取與百分比或您設定為大小限制的最大數量對應的多個設定檔。

   ![](assets/control-group.png)

* **按屬性排名**：此選項可讓您根據特定排序順序中的特定屬性排除一組設定檔。

   ![](assets/control-group2.png)

然後，定義&#x200B;**大小限制**：您必須設定如何限制從主要目標擷取的設定檔數量。

**範例**

您可以檢視記錄以檢查和識別排除的設定檔。讓我們以隨機排除五個設定檔為範例。

![](assets/control-group4.png)

傳遞準備後，您可以在以下畫面檢視排除情況：

* 傳遞儀表板中的&#x200B;**要排除** KPI，傳送前。

   ![](assets/control-group5.png)

* **排除記錄**&#x200B;顯示每個設定檔和相關的排除&#x200B;**原因**。

   ![](assets/control-group6.png)

* **排除原因**&#x200B;顯示每個類型規則之排除的設定檔數量。

   ![](assets/control-group7.png)

如需傳遞記錄的詳細資訊，請參閱本[章節](../monitor/delivery-logs.md)。

## 額外母體 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="額外母體"
>abstract="定義控制組的另一種方法是使用現有對象或定義查詢從目標中排除特定母體。"

定義控制組的另一種方法是使用現有對象或定義查詢從目標中排除特定母體。

從&#x200B;**控制組**&#x200B;定義畫面的「**額外母體**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

![](assets/control-group3.png)

* 若要使用現有對象，按一下「**選取對象**」。請參閱本[章節](add-audience.md)。

* 若要定義新查詢，請選取「**建立您自己的**」並使用規則產生器定義排除標準。請參閱本[章節](segment-builder.md)。

包含在對象中或與查詢結果相符的設定檔將從目標中排除。