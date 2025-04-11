---
audience: end-user
title: 傳送簡訊傳遞
description: 瞭解如何使用Adobe Campaign網頁版傳送簡訊
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 11%

---

# 預覽並傳送簡訊傳遞 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔離量度"
>abstract="傳遞失敗 (使用者未知、網域無效) 後被隔離的地址總數與要傳遞之訊息數量的關係。"

## 預覽您的SMS傳送 {#preview-sms}

定義訊息內容後，請使用測試設定檔來預覽及測試。 如果包含個人化內容，請使用測試設定檔資料來檢查此內容在訊息中的顯示方式。 這可確保訊息按預期顯示，且個人化資訊可正確顯示。

預覽SMS傳送的主要步驟如下。 如需如何預覽傳遞的詳細資訊，請參閱[本節](../preview-test/preview-content.md)。

1. 從您的傳遞內容頁面，使用&#x200B;**[!UICONTROL 模擬內容]**&#x200B;來預覽您的個人化內容。

   ![預覽個人化SMS內容](assets/sms_send_1.png){zoomable="yes"}

1. 按一下「**[!UICONTROL 新增測試輪廓]**」，選取一個或多個測試輪廓或輪廓。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 在右窗格中，檢視SMS傳送的預覽，其中個人化元素會以所選設定檔的資料動態取代。

   ![顯示個人化SMS傳遞的預覽窗格](assets/sms_send_3.png){zoomable="yes"}

檢閱並傳送您的SMS訊息給您的對象。

## 測試您的SMS傳送 {#test-sms}

使用&#x200B;**Adobe Campaign**，在將訊息傳送給主要對象之前先測試訊息。 此步驟會驗證您的電子郵件行銷活動並識別潛在問題。

傳送校樣對於確保傳送的品質和效率至關重要。 校樣收件者會檢閱連結、選擇退出連結和影像等各種元素，並識別轉譯、內容、個人化設定和簡訊設定中的任何錯誤。 此程式會徹底評估並最佳化您的SMS，然後再觸及主要對象。

![傳送校樣的書本圖示](../assets/do-not-localize/book.png)瞭解如何在[本節](../preview-test/test-deliveries.md)中傳送校樣。

![正在測試SMS傳遞](assets/sms_send_6.png){zoomable="yes"}

## 傳送簡訊傳遞 {#send-sms}

1. 個人化您的SMS內容後，從您的&#x200B;**[!UICONTROL 傳遞]**&#x200B;頁面按一下&#x200B;**[!UICONTROL 檢閱和傳送]**。

   ![檢閱並傳送SMS傳遞](assets/sms_send_4.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 準備]**&#x200B;並監視提供的進度和統計資料。

   如果發生錯誤，請參閱記錄檔功能表以取得有關失敗的詳細資訊。

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以繼續最後的傳送程式，以傳送訊息。

   ![傳送SMS傳遞](assets/sms_send_5.png){zoomable="yes"}

   如果已排程簡訊傳送，請按一下&#x200B;**[!UICONTROL 依排程傳送]**&#x200B;按鈕。 在[本節](../msg/gs-messages.md#schedule-the-delivery-sending)中進一步瞭解傳遞排程。

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;按鈕以確認傳送動作。

傳送傳遞後，從傳遞頁面追蹤您的KPI （關鍵績效指標）資料，並從&#x200B;**[!UICONTROL 記錄檔]**&#x200B;功能表追蹤資料。

開始使用內建報告測量訊息的影響。 [了解更多](../reporting/sms-report.md)