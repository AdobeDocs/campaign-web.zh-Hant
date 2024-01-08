---
audience: end-user
title: 簡訊通道的全域報告
description: 瞭解SMS頻道的全域報告
badge: label="有限可用性"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 4%

---

# 簡訊通道的全域報告 {#campaign-reports-sms}

「全域」報表為使用者提供管道層級流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-sms}

### 傳遞概觀 {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS 傳遞概觀"
>abstract="此 **簡訊傳送概覽** KPI會提供SMS傳送的完整摘要、詳細深入分析和特定資料。 它提供關於您傳送之效能、效益和結果的全面資訊。"

此 **[!UICONTROL 傳遞概覽]** 報告提供全面的關鍵績效指標(KPI)，深入分析訪客與每個SMS傳送的互動模式。 以下為下列量度。

![](assets/global_report_sms_delivery_overview.png)

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數佔已傳送訊息總數的百分比。

* **[!UICONTROL 點進率]**：在傳遞中至少點按一次的不同收件者百分比。

* **[!UICONTROL 錯誤]**：在傳送及自動回訪處理期間累計的錯誤數佔已傳送訊息總數的百分比。

+++

### 目標對象 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="SMS 目標族群"
>abstract="的圖表和表格 **目標人口** 呈現與您的SMS對象相關的資料，包括要傳送的訊息和排除專案的資訊。"

此 **[!UICONTROL 目標對象]** 表格和圖表會顯示每個已傳送SMS傳遞的收件者相關資料。 量度詳情如下。

![](assets/global_report_sms_targeted_audience.png)

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="簡訊傳遞統計資料"
>abstract="此 **傳遞統計資料** 報告提供所傳送SMS的完整深入分析，並提供各種量度的劃分，例如成功率、錯誤發生次數和隔離的受眾。 此詳細簡報可讓您徹底檢查SMS傳送程式的整體效能和結果。"

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

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="SMS排除原因"
>abstract="此 **排除的原因** 圖表和表格說明阻止使用者設定檔接收SMS訊息的各種原因。"

此 **[!UICONTROL 排除的原因]** 圖形和表格會顯示從目標設定檔排除的使用者設定檔無法接收簡訊傳送的原因。

錯誤型別會列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## 傳遞總處理能力 {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="SMS 傳遞輸送量"
>abstract="此 **傳遞總處理能力** 報表提供有關SMS訊息傳送系統效率的廣泛深入分析，呈現指定時間範圍內成功和錯誤率的詳細概觀。"

![](assets/global_report_sms_delivery_throughput.png)

此 **[!UICONTROL 傳遞總處理能力]** 報告提供SMS訊息傳送系統效能的全面深入分析，提供指定期間成功和錯誤率的詳細摘要。
