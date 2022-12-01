---
audience: end-user
title: 準備並傳送電子郵件
description: Campaign v8網頁檔案
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# 準備並傳送您的電子郵件 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="準備並傳送您的電子郵件"
>abstract="了解如何準備電子郵件，並進一步了解如何傳送KPI。"

>[!NOTE]
>
>本檔案正在建置中，且經常更新。 此內容的最終版本將於2023年1月推出。

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 準備傳送

在準備期間，會計算目標母體，並為目標中包含的每個設定檔產生訊息內容。 準備完成後，即可立即發送或在排程的日期和時間發送郵件。 分析期間使用的驗證規則如下 [節](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. 按一下 **準備** 按鈕。

1. 將顯示準備進度。 根據目標母體的大小，此操作可能需要一些時間。

   >[!NOTE]
   >
   >您隨時可以使用 **停止準備** 按鈕。 在準備階段期間，不會傳送任何訊息。 因此，您可以開始或停止此操作，而不會有影響任何內容的風險。

1. 準備完成後，請檢查 **已鎖定**, **交付** 和 **若要排除** KPI。 如果要傳送的訊息數量不符合您的期望，請修改您的對象並重新開始準備。

1. 按一下 **記錄檔** 按鈕並檢查是否沒有錯誤。 列出所有驗證步驟、警告和錯誤。 彩色表徵圖顯示消息類型：

   * 灰色圖示表示資訊性訊息。
   * 黃色表徵圖表示非關鍵處理錯誤。
   * 紅色圖示表示有嚴重錯誤而無法傳送傳遞。

1. 進行變更後，請重新開始準備。

準備完成後，即可傳送您的訊息。 如需詳細資訊，請參閱確認傳送。


## 傳送訊息

準備完成後，請依照下列步驟傳送訊息。

1. 按一下 **傳送按鈕** 並確認。

1. 傳送進度會與三個KPI一起顯示：傳遞、開啟、點按。

1. 按一下「確定」按鈕，完成傳送作業。

記錄檔

>[!NOTE]
>
>如果已排程訊息，則會在達到傳送時間時傳送訊息。 如需排程訊息的詳細資訊，請參閱本區段。

