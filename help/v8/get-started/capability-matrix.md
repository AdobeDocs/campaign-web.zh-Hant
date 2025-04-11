---
audience: end-user
title: Campaign Web 使用者介面/用戶端主控台功能比較表
description: Campaign Web 使用者介面支援的功能清單
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 50%

---

# Campaign Web 與 Campaign 用戶端主控台 {#capabilities-matrix}

Campaign網頁使用者介面中提供重要的Campaign功能。 此介面主要是為行銷人員設計，以便規劃、發佈和衡量其行銷活動。 本頁](../rn/whats-new.md)列出所有功能[。

根據業務和資料需求以及與其他系統的連線，在Campaign使用者端主控台中管理的Campaign平台自訂。 因此，某些設定和功能只能從Campaign使用者端主控台存取、建立或管理。 部分內容將於稍後的Campaign Web使用者介面更新中提供。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 行銷活動管理 {#campaign-mgt-capabilities}

使用Campaign Web使用者介面，您可以建立跨頻道行銷活動，如本節](../campaigns/gs-campaigns.md)所述。 [下列功能僅適用於Campaign使用者端主控台。 無法在Campaign Web使用者介面中存取，但可從[Explorer功能表](user-interface.md#user-interface-explorer)看到部分內容。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，了解如何使用這些功能。

* **行銷行事曆**。行銷活動行事曆會顯示在全域時間軸中的所有方案、計畫、行銷活動和傳遞。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#campaign-calendar){target="_blank"}
* **方案與計劃**。每個行銷活動都屬於一個方案，而該方案屬於一個計畫。 在Campaign Web使用者介面中，所有行銷活動都與預設內建計畫和方案相關聯。 您僅能透過用戶端主控台建立及管理計劃與方案。 [了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#work-with-plan-and-program){target="_blank"}
* **提供者、預算及成本管理**。 您可針對行銷活動內所執行的工作設定參與的服務提供者 (包括成本結構)，並管理每個方案與行銷活動內的預算。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=zh-Hant){target="_blank"}
* **分散式行銷** (中央/地方行銷)Adobe Campaign提供分散式行銷應用程式，用於在中央實體（總部、行銷部門等）與地方實體（銷售點、地區機構等）之間實施合作行銷活動。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hant){target="_blank"}
* **行銷資源管理** (MRM)、目標、模擬及成本控制。Adobe Campaign提供行銷資源管理(MRM)應用程式，可讓您藉由提供相關工作、預算和行銷資源的完整管理和即時追蹤，以合作模式控制行銷動作。 此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=zh-Hant){target="_blank"}
* **任務管理**。在 MRM 應用程式中，可以從行銷活動控制面板建立、指派、追蹤及監控行銷活動工作。此功能僅適用用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=zh-Hant){target="_blank"}

## 通訊通道 {#channels-capabilities}

透過Campaign Web使用者介面，您可以建立、設計和傳送&#x200B;**電子郵件**、**簡訊**、**推播通知**、**直接郵件**，並使用各種專用報告來評估其影響，如本節](../msg/gs-messages.md)詳述[。 然而，目前&#x200B;**不**&#x200B;適用以下頻道：應用程式內、LINE、呼叫中心/自訂頻道、使用 X (Twitter) 進行社交行銷。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，進一步了解這些頻道。

* **LINE 傳送訊息**。LINE是免費立即訊息、語音和視訊通話的應用程式，可在所有行動裝置和個人電腦上使用。 Adobe Campaign 僅可從用戶端主控台傳送 LINE 訊息。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=zh-Hant){target="_blank"}
* **呼叫中心和自訂管道**。呼叫中心和其他自訂管道可以在您的行銷活動環境中實作。這些管道只能在用戶端主控台中使用。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=zh-Hant#other-channels){target="_blank"}
* 搭配 X (Twitter) 進行&#x200B;**社交行銷**。透過 X (Twitter) 張貼訊息和傳送直接訊息，來與客戶互動。此功能與社交行銷附加元件一起提供，只能從使用者端主控台使用。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=zh-Hant){target="_blank"}

## 登陸頁面和網頁應用程式 {#Webapps-capabilities}

Adobe Campaign 可讓您建立、設計和共用登陸頁面。全新介面中的登陸頁面體驗已完全重新設計。在本節](../landing-pages/get-started-lp.md)中探索如何在Campaign網頁使用者介面[中建立、設計和發佈登入頁面。

因此，在Campaign使用者端主控台中，您無法編輯、更新或修改在Web介面中建立的登入頁面，反之亦然。 Campaign網頁使用者介面中無法使用下列型別的網頁應用程式。 不過，其會顯示在登陸頁面清單中。請使用提供的連結來瀏覽 Campaign Classic v7 文件，並深入了解這些網頁應用程式：

* **網頁應用程式**。Adobe Campaign可讓您使用來自資料庫的預先載入資料，以及根據連線使用者的許可權調整的內容，來建立和發佈動態和互動式網頁應用程式。 此功能僅適用用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=zh-Hant){target="_blank"}
* **網路表單**。在 Campaign Web 使用者介面中，可看到用戶端主控台中設計的網頁和登陸頁面，但無法編輯或修改。使用者端主控台網頁設計工具與隨附於Campaign Web使用者介面的登入頁面設計工具之間，有些選項可能會有所不同。 [在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hant){target="_blank"}
* **線上意見調查**。您只能從用戶端主控台建立線上意見調查和收集回答。Campaign Web使用者介面中沒有此功能。 [在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=zh-Hant){target="_blank"}

## 輪廓、測試輪廓和客群 {#profiles-audiences-capabilities}

您可以在Campaign使用者端主控台和Campaign Web使用者介面中建立、管理和更新設定檔及測試設定檔。 在一個介面中執行的所有變更都會顯示在另一個介面中。 不過，新的Campaign Web使用者介面中可能遺漏某些特定的收件者設定和進階引數。

請注意，在新的Web使用者介面中，「收件者」一詞已變更為「設定檔」，而「種子地址」現在是「測試設定檔」。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

在Campaign使用者端主控台或Adobe Experience Platform中建立的所有對象，都可以在Campaign Web使用者介面中使用。

如[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=zh-Hant#import-jobs){target="_blank"}中所述，單次匯入/匯出作業在Campaign Web使用者介面中無法使用。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## 內容設計 {#content-capabilities}

Adobe Campaign Web 使用者介面隨附全新的電子郵件設計工具，可讓您透過直覺式的拖放介面，輕鬆建立吸引人、個人化量身打造的電子郵件。無論您是從空白顯示窗開始、匯入現有內容或運用現有範本，都可以為每封電子郵件設計和調整所有內容。 [了解更多](../email/edit-content.md)

透過這個全新的使用者介面，您可以從Adobe Experience Manager管理電子郵件範本同步，並與Adobe Experience Manager as a Cloud Service整合。

請注意，Campaign Web使用者介面中暫時不提供下列功能。 使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些功能。

* **自訂個人化區塊建立功能**。除了預設的個人化區塊之外，您還可以從用戶端主控台建立自訂區塊。Campaign Web使用者介面中沒有此功能。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=zh-Hant#create-custom-personalization-blocks){target="_blank"}
* **自訂表單中的內容**。內容管理模組可讓您建立和管理表單，協助使用者在 Campaign 中建立內容。此功能僅適用於用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=zh-Hant){target="_blank"}
* **電子郵件 AMP**。AMP for Email格式可讓您在訊息中加入AMP元件，並透過豐富可行的內容改善電子郵件體驗。 此功能僅適用用戶端主控台。[在 Campaign Classic v7 文件中了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=zh-Hant){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 類型與類型規則 {#rules-capabilities}

型別是一組型別規則，在準備階段期間執行，以一次輕鬆將多個篩選規則套用至傳遞。 它們可讓行銷人員透過控制、篩選和優先處理傳送來標準化所有傳送的業務實務。

可在Campaign Web使用者介面中為傳遞或傳遞範本選取型別規則，如本節](../advanced-settings/delivery-settings.md#typology)中詳述[。 但是，規則和型別規則的建立、管理和自訂只能在Campaign使用者端主控台中使用。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解類型規則：

* 建立控制規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=zh-Hant){target="_blank"}
* 疲勞/壓力規則建立。 [了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}
* 建立篩選規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=zh-Hant){target="_blank"}
* 管理類型規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=zh-Hant){target="_blank"}
* 模擬行銷活動。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=zh-Hant){target="_blank"}
* 用於製作類型規則的 JavaScript 編碼。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant#use-cases-on-pressure-rules){target="_blank"}

## 工作流程 {#wf-capabilities}

新的 Campaign Web 使用者介面帶來重新設計的工作流程畫布介面，可供您設計和管理流程。重要工作流程活動已在新設計中提供，部分活動將在未來更新中提供。 在本節](../get-started/guardrails.md)中進一步瞭解工作流程功能，包括護欄和限制[。

請注意，下列功能僅可在 Campaign 用戶端主控台中使用：

* 工作流程中的指令碼編寫
* ETL 活動：匯出、編輯結構描述、資料載入、資料擷取、SQL 程式碼

在[這裡](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=zh-Hant){target="_blank"}的 Adobe Campaign v8 (主控台) 工作流程文件中，深入了解可用工作流程活動。

## 產品建議管理 {#offer-capabilities}

您可以在 Adobe Campaign Web 使用者介面中建立的傳遞中傳送產品建議。務必已使用&#x200B;**[!UICONTROL 互動]**&#x200B;模組，在用戶端主控台中建立這些產品建議。優惠方案設計、適用規則和優惠方案管理僅可在Campaign使用者端主控台中使用。 [了解更多](../msg/offers.md)

在 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hant){target="_blank"}中，了解如何管理產品建議目錄。

## 與 Adobe Experience Cloud 解決方案整合 {#exc-capabilities}

新的Campaign現代化UI簡化了行銷活動的設計和交付，並與其他Adobe解決方案(包括Adobe Experience Platform和Adobe Experience Manager)保持一致。

下列整合可從Adobe Campaign使用者端主控台取得，但尚未在Campaign Web使用者介面中提供。 使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些整合：

* Adobe Analytics 資料使用情況和 KPI 共用。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Experience Cloud 共用對象 (Adobe Audience Manager)。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Target 整合。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=zh-Hant){target="_blank"}
* 整合 Adobe Experience Cloud Triggers。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=zh-Hant){target="_blank"}

## 報告 {#reporting-capabilities}

新的Campaign Web使用者介面隨附一組適用於所有管道的新報告和KPI：傳遞報告、行銷活動報告和全域報告。 若要了解詳細資訊，請參閱[本章節](../reporting/gs-reports.md)

部分功能僅能從用戶端主控台取得。瀏覽提供的連結至[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hant){target="_blank"}並深入瞭解。

* 內建傳遞能力報告和收件匣轉譯。 [了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=zh-Hant){target="_blank"}
* 報告自訂。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=zh-Hant){target="_blank"}
* 描述性分析。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=zh-Hant){target="_blank"}
* 行銷活動分析/多維度資料集報告。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=zh-Hant){target="_blank"}
* 依據排程以 PDF 和 CSV 或連結形式共用報告。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=zh-Hant){target="_blank"}

## 資料模式和資料內嵌 {#data-capabilities}

Campaign Web 使用者介面不顯示下列功能。這些功能僅適用於用戶端主控台：

### 外部帳戶 {#external}

Adobe Campaign 隨附一組預先定義的外部帳戶，可與外部系統連線。作為 Campaign 系統管理員，您可以建立和管理外部帳戶。[了解更多](../administration/external-account.md)

### 結構描述建立及擴充 {#schema}

結構描述建立、修改及擴充功能僅限進階使用者使用。這些功能僅能從用戶端主控台取得。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=zh-Hant){target="_blank"}

### 工作流程資料管理功能 {#data}

資料管理結合了一套活動來解決複雜的目標定位問題，提供更有效且更靈活的工具，例如資料載入、擷取 (檔案)、更新資料、編輯結構描述或匯入/匯出技術工作流程。[探索用戶端主控台中的工作流程資料管理功能](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=zh-Hant#data-management){target="_blank"}

>[!NOTE]
>
>雖然有些活動只能在使用者端主控台中使用，但有些可在Campaign Web使用者介面中使用，例如&#x200B;**擴充**、**載入檔案**、**變更資料來源**&#x200B;或&#x200B;**變更維度**&#x200B;活動。 [在Campaign網頁使用者介面中進一步瞭解目標定位與資料管理活動](../workflows/activities/about-activities.md#targeting)

### 同盟資料存取設定 {#fda}

Campaign 設定與外部系統連線僅限進階使用者使用，且僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hant){target="_blank"}

## 核准 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="核准管理"
>abstract="核准管理僅能自用戶端控制台進行。 "

Campaign Web使用者介面不會顯示內容、傳遞、工作流程、行銷活動和目標的核准管理。 這些功能僅適用於用戶端主控台。

若要了解如何針對工作流程管理核准，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=zh-Hant){target="_blank"}。

在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=zh-Hant){target="_blank"}中瞭解如何管理行銷活動中的傳遞、內容和目標核准。

## 權限 {#permissions-capabilities}

Campaign使用者只能透過Adobe Identity Management System (IMS)，使用其Adobe ID存取Campaign Web使用者介面。 授予使用者的許可權也會套用在Campaign網頁使用者介面中。

許可權是在Adobe Admin Console和Adobe Campaign使用者端主控台中定義，如本節](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=zh-Hant)中詳細說明的[。 無法從Adobe Campaign網頁使用者介面中執行任何許可權動作。

## 監視 {#monitoring-capabilities}

Campaign平台監視功能僅在使用者端主控台和Campaign控制面板中可用。 它們不會顯示在Campaign網頁使用者介面中。

瀏覽提供的 Campaign v8 (用戶端主控台) 文件和控制面板文件連結，以了解更多資訊。

* [工作流程監視](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=zh-Hant){target="_blank"}
* [工作流程熱度圖](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=zh-Hant){target="_blank"}
* [效能監視](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=zh-Hant){target="_blank"}
* [傳遞能力監視](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=zh-Hant){target="_blank"}