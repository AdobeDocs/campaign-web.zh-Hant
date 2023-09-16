---
audience: end-user
title: 使用重複資料刪除工作流程活動
description: 瞭解如何使用重複資料刪除工作流程活動
badge: label="Beta"
source-git-commit: bf98ca98510f51fb7496a380f6547b0d3e954006
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 6%

---


# 去重複化 {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="產生補充"
>abstract="您可以產生具有剩餘母體的其他出站轉變，該母體已排除為重複。 若要這麼做，請開啟 **產生補充** 選項"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="重複資料刪除 - 重複設定"
>abstract="若要刪除傳入資料中的重複專案，請在下列欄位中定義重複資料刪除方法。 依預設，僅保留一個記錄。 您也應該根據運算式或屬性來選取重複資料刪除模式。 依預設，會隨機選取要排除在重複專案外的記錄。"

此 **重複資料刪除** 活動是 **目標定位** 活動。 此活動可讓您刪除入站活動結果中的重複專案。 此 **重複資料刪除** 活動通常用於目標定位活動之後，以及允許使用目標定位資料之活動之前。

## 設定

請依照下列步驟設定 **重複資料刪除** 活動：

1. 新增 **重複資料刪除** 活動至您的工作流程。

   ![](../assets/workflow-deduplication.png)

1. 在 **識別重複專案的欄位** 區段，按一下 **新增屬性** 按鈕來指定相同值可識別重複專案的欄位：電子郵件地址、名字、姓氏等。 欄位順序可讓您指定要先處理的欄位。

1. 選取唯一數量 **要保留的重複專案**. 此欄位的預設值為 1。如果值為 0 則可讓您保留所有重複項目。

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. 選取 **重複資料刪除方法** 若要使用：

   * **隨機選取**：隨機選取要保留在重複專案外的記錄。
   * **使用運算式**：這可讓您保留所輸入運算式的值最小或最大的記錄。 ++運算式++排序
   * **追隨值清單**：可讓您定義一或多個欄位的值優先順序。 若要定義值，請按一下 **屬性** 以選取欄位或建立運算式，然後將值新增至適當的表格。 若要定義新欄位，請按一下值清單上方的「新增」按鈕。 ++ 排序

1. 檢查 **產生補充** 選項，以利用剩餘母體。 補充包含所有重複專案。 隨後會將其他轉變新增至活動。

## 範例

