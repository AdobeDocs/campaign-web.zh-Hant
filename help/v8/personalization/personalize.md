---
title: 在 Campaign 中個人化您的內容
description: 了解如何在 Adobe Campaign Web UI 中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 551e6b9efa8b29475bd2f0a71ce016681bf70289
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 5%

---


# 個人化您的內容 {#add-personalization}

使用運算式編輯器可將個人化新增至任何傳送，可在每個欄位中使用 **[!UICONTROL 開啟個人化對話方塊]** 圖示，例如主旨行欄位，或電子郵件連結和文字/按鈕內容元件。 [瞭解新增動態內容的位置](gs-personalization.md/#access)

## 個人化語法 {#syntax}

個人化標籤一律會使用以下語法： `<%=table.field%>`. 例如，若要插入儲存在收件者表格中的收件者名稱，個人化標籤會使用&lt;%= recipient.lastName %>語法。

準備傳送時，Adobe Campaign會自動解譯這些標籤，並以指定收件者的欄位值取代。 然後在模擬您的內容時，可以檢視實體取代。

## 新增個人化標籤 {#add}

若要將個人化標籤新增至傳遞中，請使用 **[!UICONTROL 開啟個人化對話方塊]** 圖示可從文字型別編輯欄位存取，例如主旨行或SMS內文。 [瞭解新增動態內容的位置](gs-personalization.md/#access)

![](assets/perso-access.png)

運算式編輯器隨即顯示。 個人化欄位會整理成數個選單，位於畫面左側。 這些功能表可讓您存取Adobe Campaign資料庫中的所有欄位。

![](assets/perso-insert-field.png)

| 選單 | 說明 |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | 此 **[!UICONTROL 訂閱者應用程式]** 功能表會列出與應用程式訂閱者相關的所有欄位，例如使用的終端機或作業系統。 *此功能表僅供推播通知使用* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | 此 **[!UICONTROL 收件者]** 功能表會列出在收件者表格中定義的所有欄位，例如收件者的名稱、年齡或地址。 |
| ![](assets/do-not-localize/perso-message-menu.png) | 此 **[!UICONTROL 訊息]** 功能表會列出與傳送記錄檔相關的所有欄位，也就是跨所有管道傳送給收件者或裝置的所有訊息，例如與指定收件者的最後一個事件日期 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 此 **[!UICONTROL 傳遞]** 功能表會列出與執行傳送所需的引數相關的所有欄位，例如傳送頻道、標籤等。 |

>[!NOTE]
>
>依預設，每個功能表都會顯示所選表格中的所有欄位（收件者、/訊息/傳送）。 如果要包含連結至所選表格的表格欄位，請啟用 **[!UICONTROL 顯示進階屬性]** 選項的位置。

若要新增個人化欄位，請將游標置於內容內的所需位置，然後按一下+按鈕以插入該欄位。

內容準備就緒後，您可以儲存內容，並透過模擬內容來測試個人化的呈現。 在以下範例中，我們正在使用目標設定檔的名字個人化SMS訊息。

*在訊息內容中新增個人化標籤*

![](assets/perso-preview1.png)

*模擬特定測試設定檔的個人化呈現*

![](assets/perso-preview2.png)
