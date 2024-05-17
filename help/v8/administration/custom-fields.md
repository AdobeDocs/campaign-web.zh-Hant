---
title: 自訂欄位
description: 瞭解如何設定自訂欄位
hide: true
hidefromtoc: true
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 3f4b2c83b5c651e473de9e32656aaf83af6fe8c6
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# 設定自訂欄位 {#custom-fields}

自訂欄位是透過Adobe Campaign主控台新增到現成可用方案的其他屬性。 進一步瞭解 [Adobe Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

這些自訂欄位會顯示在各種畫面中，例如設定檔或測試設定檔的詳細資訊。

在Web使用者介面中，您無法建立自訂欄位，但可以修改其顯示方式。 修改會套用至所有Campaign使用者。

>[!NOTE]
>
>您必須有管理員許可權才能修改自訂欄位。

自訂欄位可用於下列結構描述：

* 收件者(nms)
* 行銷活動(nms)
* 傳遞(nms)
* 種子地址(nms)

若要設定自訂欄位，請執行下列步驟：

1. 在 **管理**，按一下 **方案**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. 找到所需的結構描述，例如 **收件者(nms)** 綱要。

   ![](assets/custom-fields2.png){zoomable="yes"}

1. 按一下 **更多動作** 按鈕並選取 **編輯自訂詳細資料**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   此 **編輯自訂詳細資料** 畫面會顯示所有自訂欄位及其型別。

   ![](assets/custom-fields4.png){zoomable="yes"}

   此畫面可讓您執行下列動作：

   * 使用向上和向下箭頭變更不同欄位的順序。
   * 將欄位設為必填：檢查 **強制** 方塊。
   * 顯示或隱藏欄位：按一下 **可見** 按鈕。
   * 新增可見度條件：按一下 **顯示條件** 按鈕並使用可用的xtk函式來撰寫xtk運算式。

1. 導覽至顯示自訂欄位的畫面。 在我們的範例中，這是設定檔詳細資訊畫面。

   ![](assets/custom-fields5.png){zoomable="yes"}
