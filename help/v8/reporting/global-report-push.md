---
audience: end-user
title: 推播通道的全域報表
description: 瞭解推播通道的全域報表
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 23%

---

# 推播通道的全域報表 {#campaign-reports-push}

全域報表為使用者提供管道層級的流量和參與量度的完整總覽。

瀏覽至&#x200B;**[!UICONTROL 報表]**&#x200B;區段內的&#x200B;**[!UICONTROL 報表]**&#x200B;功能表。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-push}

### 傳遞概觀 {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="推播傳遞概觀"
>abstract="推播&#x200B;**傳遞概觀** KPI 可對您的推播傳遞進行徹底檢查，提供詳細的洞察和特定資料。它提供了有關傳遞績效、有效性和結果的全面詳細資訊。"

**[!UICONTROL 傳遞總覽]**&#x200B;報告提供關鍵績效指標(KPI)，可提供訪客如何與每個推播通知傳遞互動的詳細資訊。 量度詳情如下。

![傳遞總覽量度，顯示與推播通知效能相關的KPI。](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++進一步瞭解傳遞概述量度。

* **[!UICONTROL 要傳遞的訊息]**：傳遞準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：與已傳送訊息總數相關的成功傳送訊息數。

* **[!UICONTROL 點按總數]**：在傳遞中至少點按一次的不同收件者總數。

* **[!UICONTROL 錯誤]**：傳遞期間累積的錯誤總數，以及相對於已傳送訊息總數，的自動傳回處理。

+++

### 目標對象 {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="推播目標群體"
>abstract="**目標群體**&#x200B;圖表和表格顯示與推播訊息對象相關的資料，顯示有關要傳遞和排除的訊息。"

針對每個已傳送的推播通知傳遞，**[!UICONTROL 目標對象]**&#x200B;表格和圖表會顯示與收件者相關的資料。 量度詳情如下。

![目標對象量度，顯示與推播通知的收件者和排除專案相關的資料。](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：傳遞準備後要傳遞的訊息總數。

* **[!UICONTROL 排除]**：套用規則時，分析期間忽略的地址總數：地址遺失、隔離、加入封鎖清單及類似原因。

+++

### 傳遞統計資料 {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="推播傳遞統計資料"
>abstract="**整體統計資料**&#x200B;報告提供有關已傳送推送播通知的資訊，包括成功率、錯誤和隔離。"

**[!UICONTROL 傳遞統計資料]**&#x200B;表格詳細說明每個推播通知傳遞的成功情況。 量度詳情如下。

![傳遞統計量度，顯示推播通知的成功率、錯誤和隔離。](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 訊息總數]**：傳遞準備後要傳遞的訊息總數。

* **[!UICONTROL 成功]**：已順利處理的訊息數與要傳遞的訊息數有關。

* **[!UICONTROL 錯誤/退信]**：傳遞期間累積的錯誤總數，以及相對於要傳遞的訊息數的自動復原處理次數。

* **[!UICONTROL 新隔離]**：在傳送失敗（無效註冊、郵件拒絕、裝載錯誤及類似原因）之後被隔離的地址總數，與要傳送的郵件數相關。

  推播通知錯誤型別列在[Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}中。

+++

### 排除的原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="推播排除的原因"
>abstract="**「排除原因」**&#x200B;圖表和表格說明阻止使用者設定檔接收推播通知的多種原因。"

排除原因&#x200B;**[!UICONTROL 圖形與表格會顯示從目標設定檔中排除的使用者設定檔無法接收訊息的原因。]**

推播通知錯誤型別列在[Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}中。

## 傳遞總處理能力 {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="傳遞輸送量報告"
>abstract="**傳遞輸送量**&#x200B;報告提供有關特定期間內整個平台推播通知傳遞輸送量的詳細資訊。"

![傳遞輸送量度，顯示特定期間推播通知的成功和錯誤率。](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

**[!UICONTROL 傳遞輸送量]**&#x200B;報表提供推播通知傳遞系統有效性的全面深入分析，提供指定期間成功率和錯誤率的詳細摘要。