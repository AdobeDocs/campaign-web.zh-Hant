---
audience: end-user
title: 簡訊通道的全域報告
description: 瞭解SMS頻道的全域報告
badge: label="可用性限制"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# 簡訊通道的全域報告 {#campaign-reports-sms}

「全域」報表為使用者提供管道層級流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-sms}

### 傳遞概觀 {#delivery-overview-sms}

此 **[!UICONTROL 傳遞概覽]** 報告提供全面的關鍵績效指標(KPI)，深入分析訪客與每個SMS傳送的互動模式。 以下為下列量度。

![](assets/global_report_sms_delivery_overview.png)

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數佔已傳送訊息總數的百分比。

* **[!UICONTROL 點進率]**：在傳遞中至少點按一次的不同收件者百分比。

* **[!UICONTROL 錯誤]**：在傳送及自動回訪處理期間累計的錯誤數佔已傳送訊息總數的百分比。

+++

### 目標對象 {#delivery-summary-sms-initial-target}

此 **[!UICONTROL 目標對象]** 表格和圖表會顯示每個已傳送SMS傳遞的收件者相關資料。 量度詳情如下。

![](assets/global_report_sms_targeted_audience.png)

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-sms-exec-stats}

此 **[!UICONTROL 傳遞統計資料]** 表格詳細說明您每次SMS傳送的成功情況。 量度詳情如下。

![](assets/global_report_sms_delivery_statistics.png)

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 訊息總數]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

  SMS錯誤型別會列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### 排除的原因 {#causes-exclusion}

此 **[!UICONTROL 排除的原因]** 圖形和表格會顯示從目標設定檔排除的使用者設定檔無法接收簡訊傳送的原因。

錯誤型別會列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## 傳遞總處理能力 {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

此報表提供指定時間範圍內傳送輸送量的完整詳細資料。
