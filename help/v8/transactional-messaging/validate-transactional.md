---
audience: end-user
title: 驗證異動訊息
description: 瞭解如何在Campaign網頁使用者介面中驗證交易式訊息
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 1%

---

# 驗證異動訊息

在建立交易式訊息期間或之後，您可能會想要使用資料範例來驗證內容。

## 模擬內容 {#simulate-content}

請依照下列步驟模擬訊息的內容：

* 確保訊息內容中的個人化路徑符合內容範例。 在下列範例中，若要顯示測試設定檔的名字，請使用路徑&#x200B;*rtEvent.ctx.basicDetails.firstName*。

  您可以修改訊息內容或內容範例，使其對齊。

  ![熒幕擷圖顯示訊息內容中的個人化路徑驗證](assets/validate-verification.png){zoomable="yes"}

* 按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕，以預覽交易式訊息與內容範例中輸入的資料。

  ![顯示[模擬內容]按鈕和預覽功能的熒幕擷圖](assets/validate-simulate.png){zoomable="yes"}

  檢閱您的內容後，按一下&#x200B;**[!UICONTROL 關閉]**&#x200B;按鈕。

* 如果您對內容進行任何變更，請確定您按一下&#x200B;**[!UICONTROL 重新發佈]**&#x200B;按鈕。

## 傳送校樣

若要測試並體驗交易式訊息透過您所選頻道（例如電子郵件、簡訊或推播通知）傳送的方式，請使用校樣功能。

在[模擬內容視窗](#simulate-content)中，按一下&#x200B;**[!UICONTROL 傳送校樣]**&#x200B;按鈕。

![在模擬內容視窗中顯示[傳送校樣]按鈕的熒幕擷圖](assets/transactional-proof.png){zoomable="yes"}

在出現的新視窗中，輸入電子郵件地址或電話號碼，視您要接收校訂的頻道而定。 輸入想要的地址後，按一下&#x200B;**[!UICONTROL 傳送校樣]**&#x200B;和&#x200B;**[!UICONTROL 確認]**&#x200B;按鈕。 此動作會傳送交易式訊息的範例，確保所有個人化、動態內容和格式正確顯示給一般使用者。

![顯示傳送證明功能與確認程式的熒幕擷圖](assets/transactional-sendproof.png){zoomable="yes"}

此步驟對於在發佈交易式訊息之前識別任何潛在問題至關重要。