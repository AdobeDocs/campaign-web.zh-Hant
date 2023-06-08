---
title: 在 Campaign 中個人化您的內容
description: 了解如何在 Adobe Campaign Web UI 中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

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

## 個人化您的電子郵件內容 {#personalize-emails}

若要個人化電子郵件內容，請在電子郵件設計工具中開啟訊息，然後：

1. 在文字區塊內按一下。
1. 在內容關聯式工具列中，選取「**[!UICONTROL 新增個人化]**」。

   ![](assets/perso-add-to-content.png)

1. 在個人化編輯器中插入收件者名稱並確認。

   ![](assets/perso-add-name.png)

   個人化屬性已新增到電子郵件內容。

   您可以模擬內容以檢查轉譯。[了解更多](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. 若要在電子郵件中新增內容區塊，請執行相同的步驟，然後從最後一個圖示選取內容區塊：

   ![](assets/perso-insert-block.png)

1. 插入後，即將內容區塊新增到電子郵件內容。在傳遞準備步驟中，個人化產生時，它會自動適應收件者設定檔。

   ![](assets/perso-content-block-in-email.png)


## 個人化您的優惠 {#personalize-offers}

您也可以在將文字類型的內容新增到優惠的表示時存取個人化編輯器。在[本章節](../content/offers.md)了解更多資訊。

