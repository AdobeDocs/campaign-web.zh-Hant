---
audience: end-user
title: Campaign Web 使用者介面/用戶端主控台功能比較表
description: Campaign Web 使用者介面支援的功能清單
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '2141'
ht-degree: 99%

---

# Campaign Web 與 Campaign 用戶端主控台 {#capabilities-matrix}

Campaign Web 使用者介面提供的主要 Campaign 功能。此介面主要設計目的是供行銷人員計劃、啟動及測量其行銷活動。 [本頁面](../rn/whats-new.md)列出所有功能。

Campaign Platform 可依據企業與資料需求自訂，且可透過 Campaign 用戶端主控台管理與其他系統的連線。因此，某些設定與功能僅能透過 Campaign 用戶端主控台來存取、建立或管理。將於稍後的 Campaign Web 使用者介面更新提供部分內容。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 行銷活動管理 {#campaign-mgt-capabilities}

您可使用 Campaign Web 使用者介面來建立跨頻道行銷活動，詳細資訊請見[本區段](../campaigns/gs-campaigns.md)。下列功能僅適用 Campaign 用戶端主控台。 這些功能無法透過 Campaign Web 使用者介面存取，但部分內容可從[瀏覽器選單](user-interface.md#user-interface-explorer)查看。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，了解如何使用這些功能。

* **行銷行事曆**。行銷活動行事曆會透過全域時間表顯示所有方案、計劃、行銷活動與傳遞。此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#campaign-calendar){target="_blank"}
* **方案與計劃**。每個行銷活動都屬於某項方案，而該方案隸屬於某項計劃。在 Campaign Web 使用者介面，所有行銷活動均關聯預設內建計劃與方案。 您僅能透過用戶端主控台建立及管理計劃與方案。 [了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#work-with-plan-and-program){target="_blank"}
* **提供者、預算與成本管理**。您可針對行銷活動內所執行的工作設定參與的服務提供者 (包括成本結構)，並管理每個方案與行銷活動內的預算。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=zh-Hant){target="_blank"}
* **分散式行銷** (中央/地方行銷)Adobe Campaign 提供分散式行銷應用程式，可供中心實體之間 (總部、行銷部門等) 實施合作行銷活動本地實體 (銷售地點、地區代理等)。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hant){target="_blank"}
* **行銷資源管理** (MRM)、目標、模擬及成本控制。Adobe Campaign 提供行銷資源管理 (MRM) 應用程式，可讓您藉由針對相關工作、預算及行銷資源提供完整管理與即時追蹤，以合作模式控制行銷動作。此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=zh-Hant){target="_blank"}
* **任務管理**。在 MRM 應用程式中，可以從行銷活動控制面板建立、指派、追蹤及監控行銷活動工作。此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=zh-Hant){target="_blank"}

## 通訊通道 {#channels-capabilities}

透過 Campaign Web 使用者介面，您可建立、設計及傳送&#x200B;**電子郵件**、**簡訊**、**推播通知**、**直接郵件**，並使用各種專用報告測量其影響，詳細資訊請參閱[本章節](../msg/gs-messages.md)。然而，目前&#x200B;**不**&#x200B;適用以下頻道：應用程式內、LINE、呼叫中心/自訂頻道、使用 X (Twitter) 進行社交行銷。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，進一步了解這些頻道。

* **LINE 傳送訊息**。LINE 是免費應用程式，可傳送即時訊息、進行語音與視訊通話，適用所有行動裝置與個人電腦。Adobe Campaign 僅可從用戶端主控台傳送 LINE 訊息。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=zh-Hant){target="_blank"}
* **呼叫中心和自訂管道**。呼叫中心和其他自訂管道可以在您的行銷活動環境中實作。這些管道只能在用戶端主控台中使用。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=zh-Hant#other-channels){target="_blank"}
* 搭配 X (Twitter) 進行&#x200B;**社交行銷**。透過 X (Twitter) 張貼訊息和傳送直接訊息，來與客戶互動。此功能隨附於社交行銷附加元件，只能從用戶端主控台取得 - [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=zh-Hant){target="_blank"}

## 登陸頁面和網頁應用程式 {#Webapps-capabilities}

Adobe Campaign 可讓您建立、設計和共用登陸頁面。全新介面中的登陸頁面體驗已完全重新設計。[在本節中](../landing-pages/get-started-lp.md)，探索如何在 Campaign Web 使用者介面中建立、設計和發佈登陸頁面。

因此，在 Campaign 用戶端主控台中，您無法編輯、更新或修改在網頁介面中建立的登陸頁面，反之亦然。Campaign Web 使用者介面中無法使用下列類型的網頁應用程式。不過，其會顯示在登陸頁面清單中。請使用提供的連結來瀏覽 Campaign Classic v7 文件，並深入了解這些網頁應用程式：

* **網頁應用程式**。Adobe Campaign 可讓您使用資料庫中的預先載入資料，以及根據連線使用者的權限調整的內容，來建立和發佈動態和互動式網頁應用程式。此功能僅適用用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=zh-Hant){target="_blank"}
* **網路表單**。在 Campaign Web 使用者介面中，可看到用戶端主控台中設計的網頁和登陸頁面，但無法編輯或修改。用戶端主控台網頁設計工具與隨附於 Campaign Web 使用者介面，有些選項可能會有所不同。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hant){target="_blank"}
* **線上意見調查**。您只能從用戶端主控台建立線上意見調查和收集回答。無法在 Campaign Web 使用者介面中使用此功能。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=zh-Hant){target="_blank"}


## 設定檔、測試設定檔和對象 {#profiles-audiences-capabilities}

您可以在 Campaign 用戶端主控台和 Campaign Web 使用者介面中，建立、管理和更新設定檔和測試設定檔。於一個 UI 中執行的所有變更，皆會顯示在另一個 UI 中。不過，新的 Campaign Web 使用者介面可能缺少某些特定的收件者設定和進階參數。

請注意，在新的網頁使用者介面中，「收件者」一詞已變更為「設定檔」，而「種子地址」現在則為「測試設定檔」

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

在 Campaign 用戶端主控台或 Adobe Experience Platform 中建立的所有對象，都可以在 Campaign Web 使用者介面中使用。

如 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=zh-Hant#import-jobs){target="_blank"}所述， 無法在 Campaign Web 使用者介面中使用單次匯入/匯出工作。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## 交易型訊息傳遞功能 {#mc-capabilities}

目前無法在新的 Campaign Web 使用者介面中，使用訊息中心產品套件隨附的交易型訊息傳遞功能。

瀏覽 [Campaign v8  (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html?lang=zh-Hant){target="_blank"}，並深入了解即時訊息傳遞功能，例如：

* 在電子郵件、簡訊和推播上的即時訊息製作和執行
* 訊息擴充和個人化
* 交易型訊息的報告和監視

## 內容設計 {#content-capabilities}

Adobe Campaign Web 使用者介面隨附全新的電子郵件設計工具，可讓您透過直覺式的拖放介面，輕鬆建立吸引人、個人化量身打造的電子郵件。無論您是從空白顯示窗開始，還是匯入現有的內容或利用現有的範本，都可針對每封電子郵件設計和改進所有內容。[了解更多](../email/edit-content.md)

透過此全新的使用者介面，您可以從 Adobe Experience Manager 管理電子郵件範本同步，並與 Adobe Experience Manager as a Cloud Service 整合。

請注意，下列功能目前無法在 Campaign Web 使用者介面中使用。使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些功能。

* **自訂個人化區塊建立功能**。除了預設的個人化區塊之外，您還可以從用戶端主控台建立自訂區塊。無法在 Campaign Web 使用者介面中使用此功能。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=zh-Hant#create-custom-personalization-blocks){target="_blank"}
* **自訂表單中的內容**。內容管理模組可讓您建立和管理表單，協助使用者在 Campaign 中建立內容。此功能僅適用於用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=zh-Hant){target="_blank"}
* **電子郵件 AMP**。電子郵件 AMP 新格式可讓您在訊息中納入 AMP 元件，並使用豐富且可執行的內容來改善電子郵件體驗。此功能僅適用用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=zh-Hant){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 類型與類型規則 {#rules-capabilities}

類型是一組類型規則，其會在準備階段執行，以便輕鬆將多個篩選規則一次套用至傳遞。因其可以控制、篩選傳送的傳遞內容，並排列其優先順序，能讓行銷人員標準化所有傳遞的業務實務。

您可以在 Campaign Web 使用者介面中，為傳遞或傳遞範本選取類型規則，如[本節中](../advanced-settings/delivery-settings.md#typology)中所詳述。不過，僅可在 Campaign 用戶端主控台中使用規則和類型規則的建立、管理和自訂功能。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解類型規則：

* 建立控制規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=zh-Hant){target="_blank"}
* 建立疲勞和壓力規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}
* 建立篩選規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=zh-Hant){target="_blank"}
* 管理類型規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=zh-Hant){target="_blank"}
* 模擬行銷活動。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=zh-Hant){target="_blank"}
* 用於製作類型規則的 JavaScript 編碼。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant#use-cases-on-pressure-rules){target="_blank"}

## 工作流程 {#wf-capabilities}

新的 Campaign Web 使用者介面帶來重新設計的工作流程畫布介面，可供您設計和管理流程。已在新設計中提供重要的工作流程活動，部分活動將在未來更新中提供。[在本節中](../get-started/guardrails.md)，深入了解工作流程功能，包括護欄和限制 

請注意，下列功能僅可在 Campaign 用戶端主控台中使用：

* 工作流程中的指令碼編寫
* ETL 活動：匯出、編輯結構描述、資料載入、資料擷取、SQL 程式碼

在[這裡](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=zh-Hant){target="_blank"}的 Adobe Campaign v8 (主控台) 工作流程文件中，深入了解可用工作流程活動。

## 優惠方案管理 {#offer-capabilities}

您可以在 Adobe Campaign Web 使用者介面中建立的傳遞中傳送優惠方案。務必已使用&#x200B;**[!UICONTROL 互動]**&#x200B;模組，在用戶端主控台中建立這些優惠方案。僅可在 Campaign 用戶端主控台中使用優惠方案設計、適用性規則和優惠方案管理功能。[了解更多](../msg/offers.md)

在 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hant){target="_blank"}中，了解如何管理優惠方案目錄。

## 與 Adobe Experience Cloud 解決方案整合 {#exc-capabilities}

這個新的 Campaign 現代 UI 簡化行銷活動的設計和傳遞，並帶來一致性，與其他 Adobe 解決方案 (包括 Adobe Experience Platform 與 Adobe Experience Manager) 相符。

下列互動功能可在 Campaign 用戶端主控台中使用，但無法在網頁使用者介面中使用。使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些整合：

* Adobe Analytics 資料使用情況和 KPI 共用。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Experience Cloud 共用對象 (Adobe Audience Manager)。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Target 整合。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=zh-Hant){target="_blank"}
* 整合 Adobe Experience Cloud Triggers。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=zh-Hant){target="_blank"}

## 報告 {#reporting-capabilities}

新 Campaign Web 使用者介面隨附一組新報告與 KPI，適用於所有頻道：傳遞報告、行銷活動報告與全域報告。 若要了解詳細資訊，請參閱[本章節](../reporting/gs-reports.md)

部分功能僅能從用戶端主控台取得。利用提供的連結來瀏覽 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hant){target="_blank"}，了解更多。

* 內建傳遞能力報告與收件匣轉譯。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=zh-Hant){target="_blank"}
* 報告自訂。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=zh-Hant){target="_blank"}
* 描述性分析。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=zh-Hant){target="_blank"}
* 行銷活動分析/多維度資料集報告。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=zh-Hant){target="_blank"}
* 依據排程以 PDF 和 CSV 或連結形式共用報告。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=zh-Hant){target="_blank"}

## 資料模式和資料內嵌 {#data-capabilities}

Campaign Web 使用者介面不顯示下列功能。這些功能僅適用於用戶端主控台：

### 外部帳戶 {#external}

Adobe Campaign 隨附一組預先定義的外部帳戶，可與外部系統連線。作為 Campaign 系統管理員，您僅能從用戶端主控台建立及管理外部帳戶。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html?lang=zh-Hant){target="_blank"}

### 綱要建立及擴充 {#schema}

方案建立、修改及擴充功能僅限進階使用者使用。這些功能僅能從用戶端主控台取得。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=zh-Hant){target="_blank"}

### 工作流程資料管理功能 {#data}

資料管理結合了一套活動來解決複雜的目標定位問題，提供更有效且更靈活的工具，例如資料載入、擷取 (檔案)、更新資料、編輯綱要或匯入/匯出技術工作流程。[探索用戶端主控台中的工作流程資料管理功能](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=zh-Hant#data-management){target="_blank"}

>[!NOTE]
>
>雖然其中的一些活動只能在用戶端主控台中使用，但有些可在 Campaign Web 使用者介面中使用，例如&#x200B;**擴充**、**載入檔案**、**變更資料來源**&#x200B;或&#x200B;**變更維度**&#x200B;活動。[在Campaign網頁使用者介面中進一步瞭解目標定位和資料管理活動](../workflows/activities/about-activities.md#targeting)

### 同盟資料存取設定 {#fda}

Campaign 設定與外部系統連線僅限進階使用者使用，且僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hant){target="_blank"}

## 核准 {#approvals-capabilities}

Campaign Web 使用者介面不會針對內容、傳遞、工作流程、行銷活動與目標顯示核准管理。這些功能僅適用於用戶端主控台。

若要了解如何針對工作流程管理核准，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=zh-Hant){target="_blank"}。


若要了解如何針對行銷活動管理傳遞、內容與目標核准，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=zh-Hant){target="_blank"}。


## 權限 {#permissions-capabilities}

Campaign 使用者僅能透過 Adobe Identity Management System (IMS) 使用其 Adobe ID 存取 Campaign Web 使用者介面。 授予使用者的權限也會套用於 Campaign  Web 使用者介面。

Adobe Admin Console 與 Adobe Campaign 用戶端控制台已定義權限，如需詳細資訊，請參閱[本章節](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=zh-Hant)。無法從 Adobe Campaign Web 使用者介面執行任何權限動作。


## 監視 {#monitoring-capabilities}

Campaign 平台監空功能僅適用於用戶端主控台與 Campaign 控制面板。 其不會出現在 Campaign Web 使用者介面中。

瀏覽提供的 Campaign v8 (用戶端主控台) 文件和控制面板文件連結，以了解更多資訊。

* [工作流程監視](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=zh-Hant){target="_blank"}
* [工作流程熱度圖](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=zh-Hant){target="_blank"}
* [效能監視](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=zh-Hant){target="_blank"}
* [傳遞能力監視](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=zh-Hant){target="_blank"}




