---
title: 在 Campaign 中個人化您的內容
description: 了解如何在 Adobe Campaign Web UI 中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 8%

---


# 個人化您的內容{#add-personalization}

可以使用運算式編輯器將個人化新增到任何傳送中。

個人化標籤一律會使用以下語法： `<%=table.field%>`例如，若要插入儲存在收件者表格中的收件者名稱，個人化標籤會使用&lt;%= recipient.lastName %>語法。

準備傳送時，Adobe Campaign會自動解譯這些標籤，並以指定收件者的欄位值取代。 然後在模擬您的內容時，可以檢視實體取代。

若要將個人化標籤新增至傳遞，請按一下可從文字型別編輯欄位（例如主旨行或簡訊內文）存取的開啟個人化對話方塊圖示。

![](assets/perso-access.png)

運算式編輯器隨即顯示。 個人化欄位會整理成三個選單，位於畫面左側。 這些功能表可讓您存取Adobe Campaign資料庫中的所有欄位。

| 選單 | 說明 |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | 此 **[!UICONTROL 收件者]** 功能表會列出在收件者表格中定義的所有欄位，例如收件者的名稱、年齡或地址。 |
| ![](assets/do-not-localize/perso-message-menu.png) | 此 **[!UICONTROL 訊息]** 功能表會列出與傳送記錄檔相關的所有欄位，也就是跨所有管道傳送給收件者或裝置的所有訊息，例如與指定收件者的最後一個事件日期 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 此 **[!UICONTROL 傳遞]** 功能表會列出與執行傳送所需的引數相關的所有欄位，例如傳送頻道、標籤等。 |

>[!NOTE]
>
>依預設，清單會顯示所選表格中的所有欄位（「收件者」、「/訊息/傳送」）。 如果要包含連結至所選表格的表格欄位，請啟用 **[!UICONTROL 顯示進階屬性]** 選項的位置。

若要新增個人化欄位，請將游標置於內容內的所需位置，然後按一下+按鈕以插入該欄位。

![](assets/perso-insert-field.png)
