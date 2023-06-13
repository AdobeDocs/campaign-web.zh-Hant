---
audience: end-user
title: 準備並傳送電子郵件
description: 了解如何使用 Campaign Web UI 準備並傳送電子郵件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 95%

---


# 準備並傳送您的電子郵件 {#prepare-send}


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

當您定義好內容、對象和排程後，您就可以準備您的訊息。在準備期間，將計算目標母體，並為目標包含的每個設定檔產生訊息內容。準備作業完成後，就可以立即或在排程的日期和時間傳送訊息。

傳遞準備期間使用的驗證規則在 [Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/validate/delivery-analysis.html){target="_blank"}.

請遵循以下步驟：

1. 按一下傳遞儀表板右上角的「**準備**」按鈕並確認。

   ![](assets/prepare.png)

   畫面會顯示準備進度。根據目標母體的大小，此操作可能需要一些時間。

   >[!NOTE]
   >
   >您可以隨時使用「**停止準備**」按鈕來停止準備作業。在準備階段，不傳送任何訊息。因此，您可以開始或停止準備而不會影響任何東西。

1. 準備作業完成後，請檢查 KPI。如果要傳送的訊息數與您的預期不符，請修改您的對象並重新開始準備。

   ![](assets/prepare2.png)

   以下是顯示的不同 KPI：

   * **目標**：目標收件者數量
   * **要傳遞**：將傳送的訊息數
   * **要排除**：類型規則排除的訊息數

1. 按一下「**記錄**」按鈕並檢查沒有錯誤。最後的記錄訊息顯示所有錯誤訊息和錯誤數量。如需詳細資訊，請參閱本[章節](delivery-logs.md)。

   ![](assets/prepare-logs.png)

如果準備作業偵測到阻止傳送傳遞的嚴重錯誤，則在傳遞儀表板中準備狀態顯示為失敗。

![](assets/prepare-error.png)

如果在準備作業後您需要對傳遞進行任何變更，則需要重新開始準備作業以使這些變更生效。

準備作業完成且沒有錯誤後，您的訊息就可以傳送了。如需詳細資訊，請參閱[本章節](#send)。

## 傳送訊息{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="已傳遞"
>abstract="已成功傳遞的訊息數。此指標每 5 分鐘會更新一次。會根據已傳送訊息的總數顯示百分比。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="開啟次數"
>abstract="開啟的訊息數。此指標每 5 分鐘會更新一次。顯示的百分比為相異開啟次數相較於已傳遞訊息數的比率。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="點按次數"
>abstract="在電子郵件中至少點按一次的收件者數量。此指標每 5 分鐘會更新一次。顯示的百分比為相異點按次數相較於已傳遞訊息數的比率。"


準備作業完成後，您現在可以傳送訊息。只有立即傳送的訊息才需要執行此步驟。如果訊息已排程，就會在定義的日期傳送。

請按照以下步驟操作：

1. 從傳遞儀表板，按一下右上角的「**傳送**」按鈕並確認。

   ![](assets/send.png)

1. 傳送進度隨即顯示。檢查顯示的 KPI。您也可以檢查記錄。如需詳細資訊，請參閱本[章節](delivery-logs.md)。

   ![](assets/send2.png)

   以下是顯示的不同 KPI：

   * **已傳遞**：已成功傳遞的訊息數。會根據已傳送訊息的總數顯示百分比。
   * **開啟**：已開啟的訊息數。顯示的百分比為相異開啟次數相較於已傳遞訊息數的比率。
   * **點按數**：在電子郵件中至少點按一次的收件者數量。顯示的百分比為相異點按次數相較於已傳遞訊息數的比率。

   >[!NOTE]
   >
   >所有指標在傳遞開始後每 5 分鐘更新一次。傳遞準備指標是即時的。

   您可以隨時暫停傳送，然後恢復傳送。如果您在傳送傳遞期間停止傳遞，則無法恢復傳送。
