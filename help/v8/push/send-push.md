---
audience: end-user
title: 傳送推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web傳送推播通知傳遞
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 13%

---

# 預覽和傳送推播通知傳遞 {#send-push}

## 預覽推播通知傳遞 {#preview-push}

定義訊息內容後，您可以利用測試設定檔來預覽和測試訊息。 如果您已包含個人化內容，則可運用測試設定檔資料，檢查此內容在訊息中的顯示方式。 這可讓您確保訊息正確轉譯，且個人化元素正確合併。

1. 從您的傳遞內容頁面，您可以使用 **[!UICONTROL 模擬內容]** 以預覽您的個人化內容。

   ![](assets/push_send_1.png)

1. 按一下「**[!UICONTROL 新增測試設定檔]**」，選取一個或多個測試設定檔或設定檔。

1. 選取測試設定檔後，按一下「**[!UICONTROL 選取]**」。

   ![](assets/push_send_5.png)

1. 在右側窗格中，您會看到電子郵件的預覽，其中個人化元素會動態地由選取的設定檔中的資料取代。

您現在可以檢閱並傳送推播通知給對象。

## 測試您的推播通知傳遞 {#test-send-sms}

使用 **Adobe Campaign**，您便能夠在將推播通知傳送給主要對象之前先測試這些通知。 此步驟對於驗證您的傳送和識別任何問題非常重要。
測試收件者可檢閱連結、影像和個人化設定等元素，確保最佳效能並偵測任何錯誤。 此程式可協助您在到達主要受眾之前調整及最佳化推播通知。

![](../assets/do-not-localize/book.png) 在此瞭解如何傳送測試推播通知 [頁面](../preview-test/proofs.md).

![](assets/push_send_6.png)

## 傳送推播通知傳遞 {#preview-send-push}

1. 個人化您的推播通知內容後，請按一下 **[!UICONTROL 檢閱並傳送]** 從您的 **[!UICONTROL 傳遞]** 頁面。

   ![](assets/push_send_2.png)

1. 按一下**[!UICONTROL 準備]**並監控提供的進度和統計資料。

   如果發生任何錯誤，請參考記錄檔功能表以取得有關失敗的詳細資訊。

   ![](assets/push_send_3.png)

1. 按一下以傳送訊息 **[!UICONTROL 傳送]** 以繼續最終的傳送程式。

1. 按一下「 」以確認傳送動作 **[!UICONTROL 傳送]** 或 **[!UICONTROL 依排程傳送]** 按鈕。

   ![](assets/push_send_4.png)

傳送後，您可以從傳送頁面追蹤KPI （關鍵績效指標）資料，以及從「記錄」選單追蹤資料。

您現在可以使用內建報告來開始衡量訊息的影響。 [了解更多](../reporting/push-report.md)
