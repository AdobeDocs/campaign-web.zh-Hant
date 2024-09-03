---
audience: end-user
title: 直接郵件報表
description: 瞭解如何存取及使用直接郵件報告
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 23%

---

# 直接郵件傳遞報告 {#direct-mail-report}

**直接郵件傳遞報告**&#x200B;提供您直接郵件傳遞的特定完整見解和資料。 其中會提供有關您的個別傳遞的效能、效益和成果的詳細資訊，為您提供全方位的概觀。

## 傳遞摘要 {#delivery-summary-direct-mail}

### 傳遞概觀 {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="傳遞概觀"
>abstract="**傳遞概觀**&#x200B;提供了關鍵績效指標 (KPI)，可讓您深入了解訪客與每次直接郵件傳遞的互動情況。這些量度概述如下。"

**[!UICONTROL 傳遞概覽]**&#x200B;提供訪客與每個直接郵件傳遞互動方式的詳細深入分析，並展示重要的關鍵績效量度(KPI)。  這些量度概述如下。

![](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++進一步瞭解傳送概述量度。

* **[!UICONTROL 要傳遞的訊息]**：傳遞準備期間處理的訊息總數。

* **[!UICONTROL 目標]**：符合直接郵件訊息目標設定檔資格的使用者設定檔數目。

* **[!UICONTROL 要排除]**：從目標設定檔中排除且不會收到直接郵件訊息的使用者設定檔數目。
+++

### 初始目標群體 {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="初始目標群體"
>abstract="**初始目標群體**&#x200B;圖表根據傳遞準備的結果顯示與收件者和訊息相關的資料。"

**[!UICONTROL 初始目標母體]**&#x200B;圖表顯示與收件者相關的資料。 量度會在傳遞準備期間計算並顯示：初始對象、要傳送的訊息數、排除的收件者數。

![](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

將滑鼠移至圖表的一部分上以顯示確切的數字。

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++深入瞭解直接郵件傳遞報告度量。

* **[!UICONTROL 初始對象]**：目標收件者的總數。

* **[!UICONTROL 要傳遞]**：傳遞準備後要傳遞的訊息總數。

* **[!UICONTROL 排除]**：從目標母體排除的收件者總數。
+++

### 傳遞統計資料 {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="傳遞統計資料"
>abstract="**傳遞統計資料**&#x200B;圖表詳細說明直接郵件傳遞成功以及發生的錯誤。"

**[!UICONTROL 傳遞統計資料]**&#x200B;圖表提供您傳遞效能的完整概觀，提供測量成功與效率的詳細量度。

![](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++進一步瞭解直接郵件行銷活動報告度量。

* **[!UICONTROL 已傳送的郵件]**：準備傳遞後要傳遞的郵件總數。

* **[!UICONTROL 成功]**：已順利處理的訊息數與要傳遞的訊息數有關。

* **[!UICONTROL 錯誤]**：傳遞期間累積的錯誤總數，以及相對於要傳遞的訊息數的自動復原處理次數。

* **[!UICONTROL 新隔離]**：在傳送失敗（使用者不明、網域無效）之後被隔離的地址總數，與要傳送的訊息數目相關。

+++

### 排除的原因 {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="傳遞排除原因"
>abstract="**排除原因**&#x200B;圖表顯示傳遞準備期間被拒絕之郵件的分佈，依每個規則進行分類。"

**[!UICONTROL 排除原因]**&#x200B;圖表提供傳遞準備過程中訊息被拒絕背後原因的詳細劃分。 此劃分會根據各種規則進行整理，提供排除訊息因素的綜合檢視。 排除規則在[Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}中有詳細說明。

![](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++深入瞭解排除量度發生的原因。

* **[!UICONTROL 隔離中的地址]**：將地址置於隔離中時產生錯誤型別。

* **[!UICONTROL 未指定地址]**：傳送傳遞時產生錯誤型別，指出地址不存在。

* **[!UICONTROL 品質不良的地址]**：當郵寄地址品質評等太低時產生的錯誤型別。

* **[!UICONTROL 已加入封鎖清單的地址]**：執行傳遞時，收件者已加入封鎖清單時產生錯誤型別。

* **[!UICONTROL Double]**：收件者因索引鍵值不唯一而被排除時產生的錯誤型別。

* **[!UICONTROL 控制組]**：收件者的地址是控制組的一部分。

* **[!UICONTROL 目標大小受限]**：已達收件者的傳遞大小上限。

+++

### 排除 {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="排除"
>abstract="**[!UICONTROL 排除]**&#x200B;表格依規則顯示傳遞準備過程中被拒絕之郵件的詳細劃分。"

**[!UICONTROL 排除專案]**&#x200B;表格提供在傳遞準備階段期間遭拒絕之訊息的深入劃分（依特定規則分類）。 此全方位的劃分可讓您清楚瞭解從傳送程式排除這些訊息的原因。

![](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

可用的量度與上述[排除原因](#direct-mail-delivery-exclusions)的量度相同。
