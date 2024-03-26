---
audience: end-user
title: 直接郵件通道的全域報告
description: 深入瞭解直接郵件通道的全域報告
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 33%

---

# 直接郵件通道的全域報告 {#global-report-direct}

直接郵件全域報表為使用者提供管道層級的流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-direct}

### 傳遞概觀 {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="傳遞概觀"
>abstract="**傳遞概觀**&#x200B;提供了關鍵績效指標 (KPI)，可讓您深入了解訪客與每次直接郵件傳遞的互動情況。這些量度概述如下。"

**[!UICONTROL 傳遞概觀]**&#x200B;提供了關鍵績效指標 (KPI)，可讓您深入了解訪客與每次直接郵件傳遞的互動情況。這些量度概述如下。

![](assets/global_report_direct_mail_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

* **[!UICONTROL 取消訂閱]**：點按取消訂閱的收件者人數。
+++

### 目標對象 {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="目標對象"
>abstract="收件者資料和訊息資訊顯示在&#x200B;**目標對象**&#x200B;圖表中，反映了傳遞準備分析。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="目標對象"
>abstract="**目標對象**&#x200B;表格根據傳遞準備程序的結果提供了收件者和對應訊息的詳細劃分。"

的表格和圖表 **[!UICONTROL 目標對象]** 顯示與收件者相關的資料，下文提供詳細量度。

![](assets/global_report_direct_mail_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="傳遞統計資料"
>abstract="**傳遞統計資料**&#x200B;圖表可讓您深入了解直接郵件傳遞的有效性，包括成功傳遞和任何發生的錯誤。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="傳遞統計資料"
>abstract="**傳遞統計資料**&#x200B;表格詳細說明直接郵件傳遞成功以及發生的錯誤。"

此 **[!UICONTROL 傳遞統計資料]** 圖表和表格提供每個直接郵件傳送成功的劃分，明細量度概述如下。

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

+++

### 排除的原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="排除"
>abstract="**排除原因**&#x200B;表格依規則顯示傳遞準備過程中被拒絕之郵件的詳細劃分。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="傳遞排除原因"
>abstract="**排除原因**&#x200B;圖表顯示傳遞準備期間被拒絕之郵件的分佈，依每個規則進行分類。"

![](assets/global_report_direct_mail_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

排除專案圖表和表格說明了從目標設定檔排除的使用者設定檔無法接收訊息的原因。

+++深入瞭解排除量度發生的原因。

* **[!UICONTROL 隔離中的地址]**：將地址置於隔離區時產生的錯誤型別。

* **[!UICONTROL 未指定地址]**：傳送傳遞時產生的錯誤型別，用以指出地址不存在。

* **[!UICONTROL 品質不良的地址]**：郵寄地址品質評等太低時產生的錯誤型別。

* **[!UICONTROL 已加入封鎖清單的地址]**：執行傳遞時將收件者加入封鎖清單時產生的錯誤型別。

* **[!UICONTROL 兩次]**：收件者因金鑰值不唯一而被排除時產生的錯誤型別。

* **[!UICONTROL 控制組]**：收件者的地址是控制組的一部分。

* **[!UICONTROL 目標大小受限]**：收件者已達到傳遞大小上限。

+++
