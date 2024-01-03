---
audience: end-user
title: 電子郵件通道的全域報告
description: 進一步瞭解電子郵件通道的全域報告
badge: label="可用性限制"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 4%

---

# 電子郵件通道的全域報告 {#global-report-direct}

「全域」報表為使用者提供管道層級流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-email}

### 傳遞概觀 {#delivery-overview-email}

此 **[!UICONTROL 傳遞概覽]** 提供關鍵績效量度(KPI)，提供訪客與每個電子郵件傳送互動的深入分析。 量度概述如下。

![](assets/global_report_email_delivery_overview.png){align="center"}

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 開啟次數總計]**：至少開啟過一次訊息的目標收件者總數。

* **[!UICONTROL 點按總數]**：在傳遞中至少點按一次的收件者總數。

* **[!UICONTROL 退回與錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

* **[!UICONTROL 取消訂閱]**：點按取消訂閱的收件者人數。
+++

### 目標對象 {#delivery-summary-email-initial-target}

的表格和圖表 **[!UICONTROL 目標對象]** 顯示與收件者相關的資料，下文提供詳細量度。

![](assets/global_report_email_targeted_audience.png){align="center"}

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-email-exec-stats}

此 **[!UICONTROL 傳遞統計資料]** 表格提供每個電子郵件傳送成功的明細，明細量度概述如下。

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

+++

### 排除的原因 {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

排除專案圖表和表格說明了從目標設定檔排除的使用者設定檔無法接收訊息的原因。

電子郵件錯誤型別列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## 傳遞總處理能力 {#delivery-throughput}

![](assets/global_report_email_delivery_throughput.png){align="center"}

此報表提供指定時間範圍內傳送輸送量的完整詳細資料。

## 無法傳遞的項目 {#non-deliverables-email}

### 依類型的錯誤劃分 {#delivery-summary-email-breakdown-per-type}

![](assets/global_report_email_breakdown_type.png){align="center"}

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

![](assets/global_report_email_breakdown_domain.png){align="center"}

此 **[!UICONTROL 每個網域的錯誤劃分]** 表格和圖表會顯示與每個網域中潛在錯誤相關的資料。 量度與以下專案通用 **[!UICONTROL 每種型別的錯誤劃分]** 表格和圖表詳見上文。

## 追蹤指標 {#tracking-indicators-email}

### 傳遞統計資料 {#delivery-summary-email-statistics}

此 **[!UICONTROL 傳遞統計資料]** 量度提供關鍵績效指標(KPI)，提供關於每個電子郵件傳送之相關資料的詳細資訊。 這些量度的進一步詳細資訊如下。

![](assets/global_report_email_delivery_statistics_tracking.png){align="center"}

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

此 **[!UICONTROL 開啟及點進率]** 表格會顯示與收件者相關的資料。 量度詳情如下。

![](assets/global_report_email_opens.png){align="center"}

+++進一步瞭解「開啟」和「點進」比率量度。

* **[!UICONTROL 已傳送]**：已傳送的訊息總數。

* **[!UICONTROL 投訴]**：此網域被回報為收件者不希望的訊息數目和百分比。

* **[!UICONTROL 不重複開啟次數]**：此網域中至少開啟過一次訊息的不同目標收件者的數目和百分比。

* **[!UICONTROL 不重複點按]**：至少點按一次相同傳遞的不同目標收件者的數目和百分比。

* **[!UICONTROL 原始反應度]**：與開啟傳送至少一次的收件者人數相比，已至少點按一次傳送的收件者人數的百分比。
+++

## URL 和點擊流量 {#url-email}

### URL和點按資料流KPI {#url-email-kpis}

此 **[!UICONTROL URL和點按流量]** 報告提供關鍵績效指標(KPI)，用於針對傳送期間收到最多點按次數的URL提供詳細分析。 量度詳情如下。

![](assets/campaign_report_email_9.png){align="center"}

+++進一步瞭解URL和點選串流量度。

* **[!UICONTROL 反應度]**：已點按傳送的目標收件者數目與已開啟傳送的目標收件者估計數目之間的比率。

* **[!UICONTROL 不重複點按]**：在傳遞中至少點選一次的不同收件者總數。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 平台平均值]** ：此平均比率顯示在每個比率（反應性、不同點按和累計點按）下，是針對過去六個月傳送的傳送進行計算。 系統只會考慮具有相同型別和相同通道的傳送。 校訂已排除。
+++

### 造訪量最高的前 10 個連結 {#top10-campaign-report-email}

此 **[!UICONTROL 前10個最常造訪的連結]** 圖表和表格包含每個連結的收件者行為可用資料。 量度詳情如下。

![](assets/global_report_email_top10.png){align="center"}

+++進一步瞭解前10個最常造訪的連結量度。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 百分比]**：與傳送互動的使用者百分比。

+++

### 特定期間的點按劃分 {#campaign-report-email-breakdown-clicks}

此 **[!UICONTROL 一段時間內點按的劃分]** 圖表包含每個連結的收件者行為可用資料。

![](assets/global_report_email_breakdown_clicks.png){align="center"}

## 使用者活動 {#user-activities-email}

此 **[!UICONTROL 使用者活動]** 報告會以圖表形式顯示開啟和點按的劃分。 此報表的量度詳情如下。

![](assets/global_report_email_user.png){align="center"}

+++進一步瞭解使用者活動量度。

* **[!UICONTROL 總點按]**：傳遞中連結的點按總數。

* **[!UICONTROL 開啟次數總計]**：此網域中至少開啟過一次訊息的不同目標收件者總數。

+++
