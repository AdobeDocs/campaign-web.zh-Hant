---
audience: end-user
title: 使用更新資料工作流程活動
description: 瞭解如何使用更新資料工作流程活動
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 18%

---

# 更新資料 {#update-data}

此 **更新資料** 活動是 **資料管理** 活動。 它可讓您對資料庫中的欄位執行大量更新。 數個選項可讓您個人化資料更新。

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## 設定更新資料活動{#update-data-configuration}

若要設定 **更新資料** 活動，從將活動新增至工作流程並定義標籤開始。

![](../assets/workflow-update-data.png)

### 作業類型

此 **作業型別** 欄位可讓您選擇要對資料庫中的資料執行的程式：

* **插入或更新**：插入資料或更新資料（如果記錄已存在於資料庫中）。
* **插入**：僅插入資料。 不更新已存在的記錄。如果已定義調和標準，則僅會新增未調和的記錄。
* **更新**：更新僅存在於資料庫中記錄的資料。
* **刪除**：刪除資料。

此 **批次大小** 欄位可讓您選取要更新的入站轉變元素數量。 例如，如果您宣告500，則處理的前500筆記錄將會更新。

### 記錄識別

您可以在此段落指定如何識別資料庫中的記錄：

* 如果資料專案與現有目標維度相關，請選取 **使用目標維度** 選項，然後從中選取 **要更新的目標維度** 欄位。
* 您也可以選取 **使用自訂連結** 並指定一或多個連結，以便識別資料庫中的資料
* 如果選取的作業型別需要更新，您必須使用 **使用調解規則** 選項。

### 要更新的欄位

在 **要更新的欄位** 區段，新增將套用更新的欄位，並視需要新增條件，以執行此更新。 若要這麼做，請使用 **出現以下條件時納入考量** 欄位。 條件會依清單順序逐一套用。使用右邊的箭頭以變更更新順序。您可以多次使用相同的目的地欄位。

您可以使用自動連結欄位 **自動對應** 按鈕。 自動連結會偵測具有相同名稱的欄位。

期間 **插入或更新** 操作型別，您可以個別選取要套用至每個欄位的操作。 若要這麼做，請選取您想要在 **作業型別** 欄位。

### 進階選項

此 **進階選項** 可讓您指定其他選項來處理資料更新及管理重複專案。

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

最後兩個選項可讓您執行特定動作：

* **產生出站轉變**：建立將在執行結束時啟用的出站轉變。 更新通常表示目標工作流程結束，因此預設不會啟用選項。

* **為拒絕產生出站轉變**：建立外站轉變，其中包含更新後未正確處理的記錄（例如，如果存在重複記錄）。 更新通常是標示目標定位工作流程的結束，因此預設不會啟動該選項。
