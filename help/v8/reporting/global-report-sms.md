---
audience: end-user
title: 簡訊通道的全域報告
description: 瞭解SMS頻道的全域報告
badge: label="有限可用性"
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 31%

---

# 簡訊通道的全域報告 {#campaign-reports-sms}

全域報表為使用者提供管道層級的流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-sms}

### 傳遞概觀 {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS 傳遞概觀"
>abstract=" **SMS 傳遞概觀** KPI 提供了 SMS 傳遞的全面摘要，提供詳細的見解和具體資料。它提供有關傳遞的績效、成效和結果的全面資訊。"

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
>abstract="**目標族群**&#x200B;的圖表和表格顯示與您的 SMS 對象相關的資料，包括有關要傳遞的訊息和排除的資訊。"

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
>abstract="**傳遞統計資料**&#x200B;報告提供了對傳送的簡訊的全面見解，提供了各種指標的詳細資訊，例如成功率、錯誤發生次數和被隔離的對象。透過這份詳細的簡報，可以全面檢查簡訊傳遞過程的整體績效和結果。"

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
>title="簡訊排除的原因"
>abstract="**排除的原因**&#x200B;圖表和表格說明了阻止使用者設定檔接收簡訊推播通知的多種原因。"

此 **[!UICONTROL 排除的原因]** 圖形和表格會顯示從目標設定檔排除的使用者設定檔無法接收簡訊傳送的原因。

錯誤型別會列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## 傳遞總處理能力 {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="簡訊傳遞輸送量"
>abstract="**傳遞輸送量**&#x200B;報告提供了有關簡訊傳遞系統效率的廣泛見解，詳細概述了指定時間範圍內的成功率和錯誤率。"

![](assets/global_report_sms_delivery_throughput.png)

此 **[!UICONTROL 傳遞總處理能力]** 報告提供SMS訊息傳送系統效能的全面深入分析，提供指定期間成功和錯誤率的詳細摘要。
