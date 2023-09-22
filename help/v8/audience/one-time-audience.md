---
audience: end-user
title: 建立傳遞的一次性對象
description: 瞭解如何建立傳遞的一次性對象。
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 建立傳遞的一次性對象 {#sone-time}

本節說明如何在建立新傳送時建立對象。 在此情況下，會使用規則產生器查詢資料庫，以定位傳送對象中要包含的收件者。

產生的對象只會用於此傳送一次。 它不會儲存在對象清單中。

定義傳送的主要目標時，您也可以：

* [選取現有對象](add-audience.md) 從 **[!UICONTROL 受眾]** 清單。
* [從外部檔案載入對象](file-audience.md) （僅適用於電子郵件）。

若要直接從傳送建立新對象，請遵循下列步驟：

1. 從傳遞建立助理的「**對象**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

   ![](assets/segment-builder0.png)

1. 選取「**建立您自己的**」。規則產生器隨即顯示。它可讓您透過篩選資料庫中包含的資料，定義傳送所定位的母體。 [瞭解如何使用規則產生器](segment-builder.md)

   ![](assets/segment-builder.png)

1. 查詢準備就緒後，按一下 **確認** 使用對象作為傳送的主要目標。

   您也可以設定控制組來測量行銷活動的影響。控制組不會收到訊息。可讓您將收到訊息之母體的行為與未收到訊息之聯絡人的行為進行比較。[了解更多](control-group.md)
