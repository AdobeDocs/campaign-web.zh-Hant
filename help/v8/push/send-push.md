---
audience: end-user
title: 傳送推播通知傳遞
description: 瞭解如何使用Adobe Campaign Web傳送推播通知傳遞
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 2%

---

# 預覽並傳送推播傳遞 {#send-push-delivery}

## 預覽推播通知傳遞 {#preview-push}

定義訊息內容後，您就可以利用測試訂閱者來預覽及測試訊息。 如果您已包含個人化內容，則可使用測試設定檔資料來檢查此內容在訊息中的顯示方式。 這可讓您確保訊息正確轉譯，且個人化元素正確合併。

預覽推播通知的主要步驟如下。 如需如何預覽傳遞的詳細資訊，請參閱[本節](../preview-test/preview-content.md)。

1. 從您的傳遞內容頁面，使用&#x200B;**[!UICONTROL 模擬內容]**&#x200B;來預覽您的個人化內容。

   ![](assets/push_send_1.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 新增訂閱者]**&#x200B;以選取一或多個設定檔，以便在推播通知內容中預覽其資料。


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. 在右窗格中，您會找到推播通知的預覽，其中個人化元素會以所選設定檔的資料動態取代。

   ![](assets/push_send_7.png){zoomable="yes"}

您現在可以檢閱並傳送推播通知給對象。

## 測試推播通知傳遞 {#test-push}

使用&#x200B;**Adobe Campaign**&#x200B;時，您可在將校樣傳送給主要對象之前先傳送校樣。 此步驟對於驗證您的傳送並識別任何問題很重要。

測試設定檔是證明收件者。 他們可以檢閱及驗證元件和設定（例如連結、影像和個人化），確保最佳效能並偵測任何錯誤。 此程式可協助您在到達主要對象之前調整並最佳化推播通知。 [瞭解如何傳送校樣](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable="yes"}

## 傳送推播通知傳遞 {#send-push}

1. 個人化您的推播通知內容後，從您的&#x200B;**[!UICONTROL 傳遞]**&#x200B;頁面按一下&#x200B;**[!UICONTROL 檢閱與傳送]**。

   ![](assets/push_send_2.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 準備]**&#x200B;並監視提供的進度和統計資料。

   如果發生任何錯誤，請參考記錄檔功能表以取得有關失敗的詳細資訊。

   ![](assets/push_send_3.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以繼續最後的傳送程式，以傳送訊息。

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以確認傳送動作。

   如果已排程推播傳遞，請按一下&#x200B;**[!UICONTROL 依排程傳送]**&#x200B;按鈕。 在[本節](../msg/gs-messages.md#schedule-the-delivery-sending)中進一步瞭解傳遞排程。

   ![](assets/push_send_4.png){zoomable="yes"}

傳送傳遞後，您可以從傳遞頁面追蹤KPI （關鍵績效指標）資料，以及從&#x200B;**[!UICONTROL 記錄檔]**&#x200B;功能表追蹤資料。

您現在可以使用內建報告來開始衡量訊息的影響。 [了解更多](../reporting/push-report.md)
