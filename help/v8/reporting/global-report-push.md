---
audience: end-user
title: 推播通道的全域報表
description: 瞭解推播通道的全域報表
badge: label="可用性限制"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 3%

---

# 推播通道的全域報表 {#campaign-reports-push}

「全域」報表為使用者提供管道層級流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-push}

### 傳遞摘要 {#delivery-overview-push}

此 **[!UICONTROL 傳遞概覽]** 報告提供關鍵績效指標(KPI)，用於提供關於訪客如何參與每個推播通知傳送的詳細資訊。 量度詳情如下。

![](assets/global_report_push_delivery_overview.png)

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 點按總數]**：在傳遞中至少點選一次的不同收件者總數。

* **[!UICONTROL 錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

+++

### 目標對象 {#delivery-summary-push-initial-target}

此 **[!UICONTROL 目標對象]** 表格和圖表會顯示每個已傳送推播通知傳遞的收件者相關資料。 量度詳情如下。

![](assets/global_report_push_targeted_audience.png)

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-push-exec-stats}

此 **[!UICONTROL 傳遞統計資料]** 表格詳細說明每個推播通知傳送的成功情況。 量度詳情如下。

![](assets/global_report_push_delivery_statistics.png)

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 訊息總數]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：傳送失敗後隔離的地址總數（無效註冊、訊息拒絕、裝載錯誤，例如） 相對於要傳遞的訊息數量。

  推播通知錯誤型別列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### 排除的原因 {#causes-exclusion}

此 **[!UICONTROL 排除的原因]** 圖形和表格會顯示使用者設定檔（從目標設定檔排除）無法接收訊息的原因。

推播通知錯誤型別列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## 傳遞總處理能力 {#delivery-throughput-sms}

![](assets/global_report_push_delivery_statistics.png)

此報表提供指定時間範圍內傳送輸送量的完整詳細資料。

