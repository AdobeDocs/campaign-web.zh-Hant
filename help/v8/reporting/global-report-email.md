---
audience: end-user
title: 電子郵件通道的全域報告
description: 進一步瞭解電子郵件通道的全域報告
exl-id: 37c575e5-fd18-4a35-a11a-922d5bda1bae
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 26%

---

# 電子郵件通道的全域報告 {#global-report-direct}

全域報表為使用者提供管道層級的流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-email}

### 傳遞概觀 {#delivery-overview-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_deliveries_overview_email"
>title="傳遞概觀"
>abstract=" **傳遞概觀**&#x200B;提供了關鍵績效指標 (KPI)，可深入了解您的對象如何與您傳送的電子郵件傳遞和行銷活動進行互動。"

此 **[!UICONTROL 傳遞概覽]** 提供關鍵績效量度(KPI)，提供訪客與每個電子郵件傳送互動的深入分析。 這些量度概述如下。

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 開啟次數總計]**：至少開啟過一次訊息的目標收件者總數。

* **[!UICONTROL 點按總數]**：在傳遞中至少點按一次的收件者總數。

* **[!UICONTROL 退回與錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

* **[!UICONTROL 取消訂閱]**：點按取消訂閱的收件者人數。
+++

### 目標對象 {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_email"
>title="初始目標對象統計資料"
>abstract="**目標對象**&#x200B;表格和圖表提供了有關收件者參與的見解，幫助您評估行銷活動和傳遞的有效性。"

的表格和圖表 **[!UICONTROL 目標對象]** 顯示與收件者相關的資料，下文提供詳細量度。

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_email_delivery_stats"
>title="傳遞統計資料"
>abstract=" **傳遞統計資料**&#x200B;圖表和表格概述了關鍵量度，包括成功傳遞、錯誤和新隔離，提供了評估傳遞效能的簡明概觀。"

此 **[!UICONTROL 傳遞統計資料]** 表格提供每個電子郵件傳送成功的明細，明細量度概述如下。

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

+++

### 排除的原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusion_email"
>title="排除的原因"
>abstract="**排除的原因**&#x200B;圖表和表格說明了傳遞準備期間郵件遭拒的具體原因，並按規則提供了詳細的劃分。"

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

排除專案圖表和表格說明了從目標設定檔排除的使用者設定檔無法接收訊息的原因。

電子郵件錯誤型別列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## 傳遞總處理能力 {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_email"
>title="傳遞總處理能力"
>abstract="此&#x200B;**傳遞總輸送量**&#x200B;提供對傳遞總輸送量的全面洞察，突顯指定時間範圍內的成功率和錯誤率。"

![](assets/global_report_email_delivery_throughput.png){zoomable=&quot;yes&quot;}{align="center"}

「傳送輸送量」報表提供傳送流程效率的深入分析，詳細說明指定時間範圍內的成功和錯誤率。

+++進一步瞭解傳送輸送量量度。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

+++

## 無法傳遞的項目 {#non-deliverables-email}

### 依類型的錯誤劃分 {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_type_email"
>title="依類型的錯誤劃分"
>abstract="詳細說明&#x200B;**依類型的錯誤劃分**&#x200B;的表格和圖表包含有關在此過程中遇到的各種錯誤類型的資訊，包括使用者未知、郵箱已滿、無效的網域等。"

![](assets/global_report_email_breakdown_type.png){zoomable=&quot;yes&quot;}{align="center"}

此 **[!UICONTROL 每種型別的錯誤劃分]** 表格和圖表會顯示與不同網域中遇到的潛在錯誤相關的資料，下文提供特定量度。

此報告中顯示的錯誤會觸發隔離程式。 有關隔離管理的詳細資訊，請參閱 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++深入瞭解每個型別量度的錯誤劃分。

* **[!UICONTROL 使用者不明]**：傳送期間產生的錯誤型別，用以指出電子郵件地址無效。

* **[!UICONTROL 無效的網域]**：傳送傳遞時產生的錯誤型別，用以指出電子郵件地址的網域錯誤或不存在。

* **[!UICONTROL 郵箱已滿]**：在嘗試傳送五次後產生的錯誤型別，以指出收件者的收件匣包含太多訊息。

* **[!UICONTROL 帳戶已停用]**：傳送傳遞時產生的錯誤型別，用以指出地址已不存在。

* **[!UICONTROL 已拒絕]**：當IAP （網際網路存取提供者）拒絕位址時產生的錯誤型別，例如在套用安全性規則（反垃圾郵件軟體）之後。

* **[!UICONTROL 無法聯絡]**：訊息發佈字串中發生的錯誤型別：SMTP轉送上的事件、暫時無法連線網域等

* **[!UICONTROL 未連線]**：錯誤型別，表示收件者的行動電話在傳送時已關閉或已中斷與網路的連線。

+++

### 依網域的錯誤劃分 {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_domain_email"
>title="依網域的錯誤劃分"
>abstract="說明&#x200B;**依網域的錯誤劃分**&#x200B;的表格和圖表顯示了與遇到的每種錯誤類型相對應的資料，並按特定網域進行分類。"

![](assets/global_report_email_breakdown_domain.png){zoomable=&quot;yes&quot;}{align="center"}

此 **[!UICONTROL 每個網域的錯誤劃分]** 表格和圖表會顯示與每個網域中潛在錯誤相關的資料。 量度與以下專案通用 **[!UICONTROL 每種型別的錯誤劃分]** 表格和圖表詳見上文。

## 追蹤指標 {#tracking-indicators-email}

### 傳遞統計資料 {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_global_delivery_statistics_summary_email"
>title="傳遞統計資料"
>abstract="**傳遞統計資料**&#x200B;關鍵績效指標 (KPI) 全面概述您的傳遞和行銷活動績效，提供有關成功傳遞、遇到的錯誤和使用者參與的見解。"

此 **[!UICONTROL 傳遞統計資料]** 量度提供關鍵績效指標(KPI)，提供關於每個電子郵件傳送之相關資料的詳細資訊。 這些量度的進一步詳細資訊如下。

![](assets/global_report_email_delivery_statistics_tracking.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 不重複開啟]**：至少開啟過一次訊息的目標收件者總數。

* **[!UICONTROL 開啟次數總計]**：此網域中至少開啟過一次訊息的不同目標收件者人數。

* **[!UICONTROL 在選擇退出連結上的點選次數]**：對取消訂閱連結的點按次數。

* **[!UICONTROL 按一下映象連結]**：點按映象頁面連結的次數。

* **[!UICONTROL 轉送次數估計]**：目標收件者轉寄的電子郵件預估數量。
+++

### 開啟及點進率 {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_open_clickthrough_email"
>title="開啟及點進率"
>abstract="**開啟及點進率**&#x200B;表格顯示了收件者對您的傳遞的參與度，展示了開啟率和點進率資料，以獲得快速且富有洞察力的概觀。"

此 **[!UICONTROL 開啟及點進率]** 表格會顯示與收件者相關的資料。 量度詳情如下。

![](assets/global_report_email_opens.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解「開啟」和「點進」比率量度。

* **[!UICONTROL 已傳送]**：已傳送的訊息總數。

* **[!UICONTROL 投訴]**：此網域被回報為收件者不希望的訊息數目和百分比。

* **[!UICONTROL 不重複開啟次數]**：此網域中至少開啟過一次訊息的不同目標收件者的數目和百分比。

* **[!UICONTROL 不重複點按]**：至少點按一次相同傳遞的不同目標收件者的數目和百分比。

* **[!UICONTROL 原始反應度]**：與開啟傳送至少一次的收件者人數相比，已至少點按一次傳送的收件者人數的百分比。
+++

## URL 和點擊流量 {#url-email}

### URL 和點按資料流 KPI {#url-email-kpis}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_clickstreams_email"
>title="URL 和點擊流量"
>abstract="**URL 和點按資料流**&#x200B;報告提供了重要的關鍵績效指標 (KPI)，詳細說明傳遞期間點擊次數最多的 URL。"

此 **[!UICONTROL URL和點按流量]** 報告提供關鍵績效指標(KPI)，用於針對傳送期間收到最多點按次數的URL提供詳細分析。 量度詳情如下。

![](assets/campaign_report_email_9.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解URL和點選串流量度。

* **[!UICONTROL 反應度]**：已點按傳送的目標收件者數目與已開啟傳送的目標收件者估計數目之間的比率。

* **[!UICONTROL 不重複點按]**：在傳遞中至少點選一次的不同收件者總數。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 平台平均值]** ：此平均比率顯示在每個比率（反應性、不同點按和累計點按）下，是針對過去六個月傳送的傳送進行計算。 系統只會考慮具有相同型別和相同通道的傳送。 校訂已排除。
+++

### 造訪量最高的前 10 個連結 {#top10-global-report-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_top10_email"
>title="造訪量最高的前 10 個連結"
>abstract="**造訪量最高的 10 個連結**&#x200B;圖表和表格顯示了收件者與每個連結互動的全面資料。"

此 **[!UICONTROL 前10個最常造訪的連結]** 圖表和表格包含每個連結的收件者行為可用資料。 量度詳情如下。

![](assets/global_report_email_top10.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解前10個最常造訪的連結量度。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 百分比]**：與傳送互動的使用者百分比。

+++

### 特定期間的點按劃分 {#global-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_click_breakdown_email"
>title="特定期間的點按劃分"
>abstract="**特定期間的點按劃分**&#x200B;圖表提供了收件者在指定時間範圍內如何與連結互動的完整檢視。"

此 **[!UICONTROL 一段時間內點按的劃分]** 圖表包含每個連結的收件者行為可用資料。

![](assets/global_report_email_breakdown_clicks.png){zoomable=&quot;yes&quot;}{align="center"}

## 使用者活動 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_user_activities_email"
>title="使用者活動"
>abstract="**使用者活動**&#x200B;的圖形表示提供了收件者互動的詳細劃分，透過資訊豐富的圖表格式描繪了開啟和點按數。"

此 **[!UICONTROL 使用者活動]** 報告會以圖表形式顯示開啟和點按的劃分。 此報表的量度詳情如下。

![](assets/global_report_email_user.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解使用者活動量度。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 開啟次數總計]**：此網域中至少開啟過一次訊息的不同目標收件者總數。

+++
