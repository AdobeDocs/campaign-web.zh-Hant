---
audience: end-user
title: 監控傳遞記錄
description: 了解如何監控傳遞記錄
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 71%

---

# 監控傳遞記錄 {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="傳遞記錄"
>abstract="傳遞記錄顯示傳送作業的詳細資料。其中會顯示傳送的詳細資料、已排除的目標、原因，以及開啟和點按數等追蹤資訊。"

在準備傳遞並按一下&#x200B;**傳送**&#x200B;按鈕後，請瀏覽至傳遞記錄檔以檢查警告、錯誤、狀態、排除和追蹤資料。 可直接從訊息儀表板存取這些記錄。其中會顯示傳送的詳細資料、已排除的目標、原因，以及開啟和點按數等追蹤資訊。

若要檢視記錄，請存取您的傳遞儀表板，然後按一下「**記錄**」按鈕。

可使用下列標籤：

* [記錄](#logs-tab)
* [傳遞](#deliveries-tab)
* [排除](#exclusion-tab)
* [排除原因](#exclusion-causes)
* [被追蹤的 URL](#tracked-urls)
* [追蹤](#tracking)

## 記錄 {#logs-tab}

「**記錄**」索引標籤包含與傳遞和校訂相關的所有訊息。特定圖示可讓您識別錯誤或警告。

列出所有驗證步驟、警告和錯誤。 彩色圖示顯示訊息類型：

* 灰色圖示表示資訊類訊息。
* 黃色圖示表示非嚴重的處理錯誤。
* 紅色圖示表示嚴重錯誤，無法傳送傳遞。 必須修正嚴重錯誤，才能傳送傳遞。

![](assets/logs.png){zoomable="yes"}


## 傳遞 {#deliveries-tab}

「**傳送記錄**」索引標籤提供此傳遞每次發生的歷史記錄。已傳送訊息的清單及其狀態會儲存在此處。它可讓您檢視每個收件者的傳送狀態。

![](assets/logs2.png){zoomable="yes"}

## 排除 {#exclusion-tab}

「**排除記錄**」索引標籤會列出已從目標排除的所有訊息，以及指定傳送失敗的原因。

![](assets/logs3.png){zoomable="yes"}

## 排除原因 {#exclusion-causes-tab}

針對每個可能的原因，**排除原因**&#x200B;索引標籤會顯示已從目標排除的訊息數目。

![](assets/logs4.png){zoomable="yes"}

## 被追蹤的 URL {#tracked-urls-tab}

**追蹤的URL**&#x200B;索引標籤會重新分組已傳送訊息中包含的URL，包括其URL型別和來源URL。

![](assets/logs5.png){zoomable="yes"}

## 追蹤 {#tracking-tab}

「**追蹤**」索引標籤會列出此傳遞的追蹤歷史記錄。此索引標籤會顯示已傳送之訊息的追蹤資料，即 Adobe Campaign 追蹤的所有 URL 主體。


![](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>如果未啟用傳遞追蹤，則不會顯示此索引標籤。