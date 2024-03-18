---
audience: end-user
title: 簡訊頻道的行銷活動報告
description: 瞭解簡訊頻道的行銷活動報告
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 20%

---

# 簡訊頻道的行銷活動報告 {#campaign-reports-sms-channel}

每個行銷活動報告都會分成不同的Widget，詳細說明行銷活動的成功和錯誤。 SMS頻道的報表和量度詳情如下。 瞭解如何在中存取您的行銷活動報告 [此頁面](campaign-reports.md).

## 傳遞摘要 {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="傳遞概觀"
>abstract="**傳遞概觀**&#x200B;報告可提供關鍵績效指標 (KPI)，其中包含訪客參與 SMS 傳遞的詳細資訊。"


此 **[!UICONTROL 傳遞概覽]** 報告提供關鍵績效指標(KPI)，這些指標提供關於訪客如何與您的SMS傳送互動的詳細資訊。 量度詳情如下。

![](assets/campaign_report_sms_1.png){zoomable=&quot;yes&quot;}

+++進一步瞭解簡訊行銷活動報告量度。

* **[!UICONTROL 已傳送總數]**：在傳送準備期間處理的訊息總數。

* **[!UICONTROL 已傳遞]**：成功傳送的訊息數，與已傳送訊息總數相關。

* **[!UICONTROL 錯誤]**：與已傳送訊息總數相關的傳送和自動回訪處理期間累計的錯誤總數。

* **[!UICONTROL 不同點按次數]**：在傳遞中至少點選一次的不同收件者總數。

+++


### 初始目標對象統計資料 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="初始目標對象統計資料"
>abstract="**初始目標對象統計資料**&#x200B;表可顯示與您收件者相關的資料"

此 **[!UICONTROL 初始目標對象統計資料]** 表格會顯示與收件者相關的資料。 量度詳情如下。


![](assets/campaign_report_sms_2.png){zoomable=&quot;yes&quot;}

+++進一步瞭解簡訊行銷活動報告量度。

* **[!UICONTROL 初始對象]**：目標收件者總數。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 被規則拒絕]**：套用規則時分析期間忽略的地址總數：地址遺失、已隔離、已加入封鎖清單等。

+++


### 執行統計資料 {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="執行統計資料"
>abstract="**執行統計資料**&#x200B;資料表詳細說明您的傳遞成功：要傳遞的訊息、成功、錯誤和新隔離。"


此 **[!UICONTROL 執行統計資料]** 表格詳細說明您的傳送是否成功。 量度詳情如下。


![](assets/campaign_report_sms_3.png){zoomable=&quot;yes&quot;}

+++進一步瞭解簡訊行銷活動報告量度。

* **[!UICONTROL 要傳遞的訊息]**：準備傳送後要傳送的訊息總數。

* **[!UICONTROL 成功]**：成功處理的訊息數與要傳送的訊息數相關。

* **[!UICONTROL 錯誤]**：與要傳送的訊息數量相關的傳送和自動復原處理期間累計的錯誤總數。

* **[!UICONTROL 新隔離]**：與要傳送的訊息數量相關的傳送失敗（使用者未知、網域無效）後隔離的地址總數。

  SMS錯誤型別會列於 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### 產生的點按資料流 {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="產生的點按資料流"
>abstract="**產生的點按資料流**&#x200B;資料表顯示收件者如何與您的傳遞互動的相關可用資料。"

此 **[!UICONTROL 產生的點按資料流]** 表格會顯示與收件者與傳遞互動的相關資料。 量度詳情如下。

![](assets/campaign_report_sms_4.png){zoomable=&quot;yes&quot;}

+++進一步瞭解簡訊行銷活動報告量度。

* **[!UICONTROL 不同點按次數]**：在傳遞中至少點選一次的不同收件者總數。

* **[!UICONTROL 點按次數]**：傳遞中連結的點按總數。

* **[!UICONTROL 反應度]**：已點按傳送的目標收件者數目與已開啟傳送的目標收件者估計數目之間的比率。

+++
