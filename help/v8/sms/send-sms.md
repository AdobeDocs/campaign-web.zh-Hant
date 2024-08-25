---
audience: end-user
title: 傳送簡訊傳遞
description: 瞭解如何使用Adobe Campaign網頁版傳送簡訊
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 14%

---

# 預覽並傳送簡訊傳遞 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔離量度"
>abstract="傳遞失敗 (使用者未知、網域無效) 後被隔離的地址總數與要傳遞之訊息數量的關係。"

## 預覽您的SMS傳送{#preview-sms}

定義訊息內容後，您就可以使用測試設定檔來預覽及測試。 如果您已包含個人化內容，則可使用測試設定檔資料來檢查此內容在訊息中的顯示方式。 這可讓您確保訊息如預期顯示，且任何個人化資訊皆正確顯示。

預覽SMS傳送的主要步驟如下。 如需如何預覽傳遞的詳細資訊，請參閱[本節](../preview-test/preview-content.md)。

1. 從您的傳遞內容頁面，使用&#x200B;**[!UICONTROL 模擬內容]**&#x200B;來預覽您的個人化內容。

   ![](assets/sms_send_1.png){zoomable="yes"}

1. 按一下「**[!UICONTROL 新增測試設定檔]**」，選取一個或多個測試設定檔或設定檔。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 在右窗格中，您會找到SMS傳送的預覽，其中個人化元素會以所選設定檔的資料動態取代。

   ![](assets/sms_send_3.png){zoomable="yes"}

您現在可以檢閱您的簡訊訊息並將其傳送給您的客群。

## 測試您的SMS傳送 {#test-sms}

透過&#x200B;**Adobe Campaign**，您可以在傳送訊息給主要對象之前先測試訊息，此為驗證電子郵件促銷活動及識別潛在問題的必要步驟。

傳送校樣是確保傳送品質和有效性的重要步驟。 校樣收件者可以檢閱連結、選擇退出連結和影像等各種元素，並識別轉譯、內容、個人化設定和簡訊設定中的任何錯誤。 此程式可協助您在到達主要受眾之前完整評估及最佳化簡訊。

![](../assets/do-not-localize/book.png)瞭解如何在[本節](../preview-test/test-deliveries.md)中傳送校樣。

![](assets/sms_send_6.png){zoomable="yes"}

## 傳送簡訊傳遞 {#send-sms}

1. 個人化您的SMS內容後，從您的&#x200B;**[!UICONTROL 傳遞]**&#x200B;頁面按一下&#x200B;**[!UICONTROL 檢閱和傳送]**。

   ![](assets/sms_send_4.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 準備]**&#x200B;並監視提供的進度和統計資料。

   如果發生任何錯誤，請參考記錄檔功能表以取得有關失敗的詳細資訊。

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以繼續最後的傳送程式，以傳送訊息。

   ![](assets/sms_send_5.png){zoomable="yes"}

   如果已排程簡訊傳送，請按一下&#x200B;**[!UICONTROL 依排程傳送]**&#x200B;按鈕。 在[本節](../msg/gs-messages.md#schedule-the-delivery-sending)中進一步瞭解傳遞排程。


1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;按鈕以確認傳送動作。

傳送傳遞後，您可以從傳遞頁面追蹤KPI （關鍵績效指標）資料，以及從&#x200B;**[!UICONTROL 記錄檔]**&#x200B;功能表追蹤資料。

您現在可以使用內建報告來開始衡量訊息的影響。 [了解更多](../reporting/sms-report.md)
