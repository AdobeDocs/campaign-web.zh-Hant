---
audience: end-user
title: 建立傳遞的一次性對象
description: 瞭解如何建立傳遞的一次性對象。
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 13%

---

# 建立一次性客群 {#one-time}

本節說明如何在建立新傳送時建立對象。 在此案例中，透過使用查詢模組化工具查詢資料庫，以傳送對象中包含的設定檔為目標。 產生的對象只會用於此傳送一次，不會儲存在對象清單中。

定義傳送的主要目標時，您也可以：
* [從&#x200B;**[!UICONTROL 對象]**&#x200B;清單中選取現有的對象](add-audience.md)。
* [從外部檔案載入對象](file-audience.md) （僅適用於電子郵件）。

若要建立傳送的一次性新對象，請遵循下列步驟：

1. 從傳遞建立助理的「**客群**」區段，按一下「**[!UICONTROL 選取客群]**」按鈕。

   [熒幕擷圖顯示傳送建立助理的「對象」區段，其中「選取對象」按鈕反白顯示](assets/segment-builder0.png){zoomable="yes"}

1. 選取&#x200B;**建立您自己的**&#x200B;以開啟查詢模型工具。 查詢建模器可讓您透過篩選資料庫中包含的資料來定義目標母體。 [瞭解如何使用查詢模型工具](../query/query-modeler-overview.md)。

   [熒幕擷圖顯示查詢模組化介面](assets/query-modeler.png){zoomable="yes"}

1. 查詢準備就緒後，請按一下&#x200B;**確認**，使用產生的對象作為傳遞的主要目標。

   您也可以設定控制組來測量行銷活動的影響。控制組未收到訊息。 這可讓您比較收到訊息的母體的行為與未收到訊息的連絡人的行為。 [了解更多](control-group.md)。