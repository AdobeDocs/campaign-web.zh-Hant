---
audience: end-user
title: 準備並傳送電子郵件
description: 了解如何使用Campaign網頁UI準備和傳送電子郵件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 4%

---

# 準備並傳送您的電子郵件 {#prepare-send}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="準備並傳送您的電子郵件"
>abstract="了解如何準備電子郵件，並進一步了解如何傳送KPI。"

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 準備傳送{#prepare}

定義內容、對象和排程後，即可準備訊息。 在準備期間，會計算目標母體，並為目標中包含的每個設定檔產生訊息內容。 準備完成後，即可立即發送或在排程的日期和時間發送郵件。 分析期間使用的驗證規則於 [Campaign Classicv7檔案](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies){target="_blank"}.

請遵循以下步驟：

1. 在傳送控制面板中，按一下 **準備** 按鈕，然後確認。

   ![](assets/prepare.png)

   將顯示準備進度。 根據目標母體的大小，此操作可能需要一些時間。

   >[!NOTE]
   >
   >您隨時可以使用 **停止準備** 按鈕。 在準備階段期間，不會傳送任何訊息。 因此，您可以開始或停止此操作，而不會有影響任何內容的風險。

1. 準備完成後，檢查KPI。 如果要傳送的訊息數量不符合您的期望，請修改您的對象並重新開始準備。

   ![](assets/prepare2.png)

   以下是顯示的不同KPI:

   * **已鎖定**:目標收件者人數
   * **交付**:要傳送的訊息數
   * **若要排除**:類型規則排除的訊息數

1. 按一下 **記錄檔** 按鈕並檢查是否沒有錯誤。 最後一條日誌消息顯示所有錯誤消息和錯誤數。 如需詳細資訊，請參閱[本區段](delivery-logs.md)。

   ![](assets/prepare-logs.png)

如果準備作業偵測到無法傳送傳送的重大錯誤，準備狀態在傳送控制面板中顯示為失敗。

![](assets/prepare-error.png)

如果您在準備後需要對傳送進行任何變更，則需要重新開始準備，以便將這些變更納入考量。

準備完成且無錯誤後，即可傳送您的訊息。 如需詳細資訊，請參閱[本區段](#send)。

## 傳送訊息{#send}

準備完成後，您現在可以傳送訊息。 只有立即傳送的訊息才需要此步驟。 如果已排程訊息，則會在定義的日期傳送。

請依照下列步驟操作：

1. 在傳送控制面板中，按一下 **傳送** 按鈕並確認。

   ![](assets/send.png)

1. 會顯示傳送進度。 檢查顯示的KPI。 您也可以檢查記錄。 如需詳細資訊，請參閱[本區段](delivery-logs.md)。

   ![](assets/send2.png)

   以下是顯示的不同KPI:

   * **傳遞**:已成功傳送的郵件數。 顯示的百分比是根據已傳送訊息的總數。
   * **開啟**:已開啟訊息的數量。 顯示的百分比是不同開啟次數與已傳送訊息數量的比率。
   * **點按次數**:在電子郵件中至少按一下一次的收件者人數。 顯示的百分比是不同點按次數與已傳送訊息數量的比率。

   >[!NOTE]
   >
   >此 **開啟** 和 **點按次數** 指標會在5分鐘後更新。

   您可以隨時暫停傳送，然後繼續。 如果您在傳送時停止傳送，則無法繼續。
