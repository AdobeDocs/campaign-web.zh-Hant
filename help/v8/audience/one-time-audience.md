---
audience: end-user
title: 建立傳遞的一次性對象
description: 瞭解如何建立傳遞的一次性對象。
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 31%

---

# 建立一次性對象 {#one-time}

本節說明如何在建立新傳送時建立對象。 在此情況下，透過使用查詢模組化工具查詢資料庫，會定位要包含在傳送對象中的設定檔。

產生的對象只會用於此傳送一次。 它不會儲存在對象清單中。

定義傳送的主要目標時，您也可以：

* [選取現有對象](add-audience.md) 從 **[!UICONTROL 受眾]** 清單。
* [從外部檔案載入對象](file-audience.md) （僅適用於電子郵件）。

若要直接從傳送建立新對象，請遵循下列步驟：

1. 從傳遞建立助理的「**對象**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. 選取「**建立您自己的**」。此時會顯示查詢建模器。 它可讓您透過篩選資料庫中包含的資料，定義傳送所定位的母體。 [瞭解如何使用查詢模型工具](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. 查詢準備就緒後，按一下 **確認** 使用對象作為傳送的主要目標。

   您也可以設定控制組來測量行銷活動的影響。控制組不會收到訊息。可讓您將收到訊息之母體的行為與未收到訊息之聯絡人的行為進行比較。[了解更多](control-group.md)
