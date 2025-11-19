---
audience: end-user
title: 簡訊傳遞報告
description: 瞭解如何存取及使用簡訊傳遞報告
exl-id: 153d3a85-0d39-42db-9906-1e7f2d1d5bae
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 32%

---

# 簡訊傳遞報告 {#sms-report}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_sms"
>title="報告傳送"
>abstract="報告中的「**傳送**」標籤可讓您深入了解訪客與您傳遞的互動，以及他們可能遇到的任何潛在錯誤。"

**SMS傳送概述**&#x200B;提供您的SMS傳送的詳細摘要，提供廣泛的深入分析和特定資料。 其中包含您傳送的效能、有效性和結果的全面資訊。

## 傳遞摘要 {#delivery-summary}

### 傳遞概觀 {#sms-delivery-overview}

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="SMS 傳遞概觀"
>abstract="**SMS 傳遞概觀** 呈現 SMS 傳遞的全面概觀，提供廣泛的深入見解和特定資料。它提供有關傳遞的績效、成效和結果的全面資訊。"

**[!UICONTROL 傳遞總覽]**&#x200B;報告提供關鍵績效指標(KPI)，可提供成功和錯誤率的詳細資訊，以及訪客如何與您的SMS訊息互動。

![說明：此影像顯示傳遞概述報告，其中包括成功率、錯誤率和訪客參與度等KPI。](assets/reporting_sms_3.png){zoomable="yes"}

+++進一步瞭解SMS傳送報告度量。

* **[!UICONTROL 傳送的總數]**：傳遞準備期間處理的訊息百分比與總數。

* **[!UICONTROL 成功]**：成功傳送的訊息百分比和數目（相對於已傳送的訊息總數）。

* **[!UICONTROL 點進率]**：與您SMS傳送中所含連結互動的使用者百分比與人數。

* **[!UICONTROL 錯誤]**：傳遞期間發生的錯誤百分比和錯誤總數，使其無法傳送至設定檔。

+++

### 目標群體 {#sms-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_targeted_population"
>title="SMS 目標群體"
>abstract="**目標群體**&#x200B;圖表和資料表顯示與您的 SMS 對象相關的資料：要傳遞的訊息和排除項目。"

**目標母體**&#x200B;圖表和表格會顯示與您的對象相關的資料。 量度詳情如下。

![說明：此影像顯示目標母體圖形和表格，其中包含要傳遞的訊息和排除等量度。](assets/reporting_sms_4.png){zoomable="yes"}

+++進一步瞭解SMS傳送報告度量。

* **[!UICONTROL 要傳遞]**：傳遞準備期間處理的訊息總數和百分比率。

* **[!UICONTROL 排除專案]**：已從分析中排除的設定檔數目和百分比率。
+++

### 整體統計資料 {#sms-delivery-overall}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_overall_stats"
>title="SMS 整體統計資料"
>abstract="**整體統計資料**&#x200B;報告顯示已傳送的 SMS 的資料：成功、錯誤和隔離。"

**整體統計資料**&#x200B;報告會顯示已傳送SMS訊息的資料。 量度詳情如下。

![說明：此影像顯示整體統計報表，其中包含成功率、錯誤和隔離等量度。](assets/reporting_sms_5.png){zoomable="yes"}

+++進一步瞭解SMS傳送報告度量。

* **[!UICONTROL 成功]**：已成功處理的訊息數目和百分比率。

* **[!UICONTROL 錯誤]**：傳遞期間發生的錯誤總數和百分比，無法傳送訊息給特定設定檔。

* **[!UICONTROL 新隔離]**：已排除並新增至隔離的設定檔數目和百分比率。
+++

### 排除 {#sms-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sms_exclusions"
>title="SMS 排除項目"
>abstract="**「排除」**&#x200B;圖表和表格顯示多種原因，禁止從目標設定檔中排除的使用者設定檔接收訊息。"

**[!UICONTROL 排除專案]**&#x200B;圖表和表格會顯示使用者設定檔無法接收訊息的原因，這些設定檔已從目標設定檔中排除。 排除規則在[Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){_blank}中有詳細說明。

![說明：此影像顯示排除專案圖表和表格，詳細說明拒絕使用者設定檔接收訊息的原因。](assets/reporting_sms_6.png){zoomable="yes"}

## 傳遞總處理能力 {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_sms"
>title="簡訊傳遞輸送量"
>abstract="**傳遞輸送量**&#x200B;報告提供有關特定期間內傳遞輸送量的詳細資訊。用於測量訊息傳遞速度的主要量度是每小時傳送的訊息數。"

此報表提供有關指定時間範圍內傳送輸送量的詳細資訊。 用於測量訊息傳遞速度的主要量度是每小時傳送的訊息數。

![說明：此影像顯示傳遞輸送量報告，其中包含指定時間範圍內每小時傳送的訊息數等量度。](assets/reporting_sms_2.png){zoomable="yes"}