---
audience: end-user
title: 直接郵件通道的全域報告
description: 深入瞭解直接郵件通道的全域報告
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 4%

---

# 直接郵件通道的全域報告 {#global-report-direct}

「全域」報表為使用者提供管道層級流量和參與量度的完整總覽。

導覽至 **[!UICONTROL 報表]** 功能表中的 **[!UICONTROL 報告]** 區段。 您可以根據報表日期、資料夾或規則來篩選資料。 [了解更多](global-reports.md)

## 傳遞摘要 {#delivery-summary-direct}

### 傳遞概觀 {#delivery-overview-direct}

此 **[!UICONTROL 傳遞概覽]** 提供關鍵績效量度(KPI)，提供訪客與每個電子郵件傳送互動的深入分析。 量度概述如下。

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

* **[!UICONTROL 取消訂閱]**：點按取消訂閱的收件者人數。
+++

### 目標對象 {#delivery-summary-direct-initial-target}

的表格和圖表 **[!UICONTROL 目標對象]** 顯示與收件者相關的資料，下文提供詳細量度。

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++深入瞭解鎖定目標對象量度。

* **[!UICONTROL 目標對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 排除]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++

### 傳遞統計資料 {#delivery-summary-direct-exec-stats}

此 **[!UICONTROL 傳遞統計資料]** 表格提供每個直接郵件傳送成功的明細，明細量度概述如下。

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++進一步瞭解傳遞統計量度。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤/退回]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

+++

### 排除的原因 {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

排除專案圖表和表格說明了從目標設定檔排除的使用者設定檔無法接收訊息的原因。

## 傳遞總處理能力 {#delivery-throughput}

此報表提供指定時間範圍內傳送輸送量的完整詳細資料。 用來測量訊息傳送速度的關鍵量度是每小時傳送的訊息數。

## 無法傳遞的項目 {#non-deliverables-direct}

### 依類型的錯誤劃分 {#delivery-summary-direct-breakdown-per-type}

此 **[!UICONTROL 每種型別的錯誤劃分]** 表格和圖表會顯示與不同網域中遇到的潛在錯誤相關的資料，下文提供特定量度。

此報告中顯示的錯誤會觸發隔離程式。 有關隔離管理的詳細資訊，請參閱 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++深入瞭解每個型別量度的錯誤劃分。

* **[!UICONTROL 使用者不明]**：傳送期間產生的錯誤型別，用以指出位址無效。

* **[!UICONTROL 無效的網域]**：傳送傳遞時產生的錯誤型別，用以指出位址的網域錯誤或不存在。

* **[!UICONTROL 郵箱已滿]**：在嘗試傳送五次後產生的錯誤型別，以指出收件者的收件匣包含太多訊息。

* **[!UICONTROL 帳戶已停用]**：傳送傳遞時產生的錯誤型別，用以指出地址已不存在。

* **[!UICONTROL 已拒絕]**：當IAP （網際網路存取提供者）拒絕位址時產生的錯誤型別，例如在套用安全性規則（反垃圾郵件軟體）之後。

* **[!UICONTROL 無法聯絡]**：訊息發佈字串中發生的錯誤型別：SMTP轉送上的事件、暫時無法連線網域等

* **[!UICONTROL 未連線]**：錯誤型別，表示收件者的行動電話在傳送時已關閉或已中斷與網路的連線。

+++

### 依網域的錯誤劃分 {#delivery-summary-email-breakdown-per-domain}

此 **[!UICONTROL 每個網域的錯誤劃分]** 表格和圖表會顯示與每個網域中潛在錯誤相關的資料。 量度與以下專案通用 **[!UICONTROL 每種型別的錯誤劃分]** 表格和圖表詳見上文。

