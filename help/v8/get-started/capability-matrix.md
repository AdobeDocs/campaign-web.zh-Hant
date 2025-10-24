---
audience: end-user
title: Campaign Web 使用者介面/用戶端主控台功能比較表
description: Campaign Web 使用者介面支援的功能清單
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '2134'
ht-degree: 97%

---

# Campaign Web 與 Campaign 用戶端主控台 {#capabilities-matrix}

Campaign Web 使用者介面可提供主要的 Campaign 功能。此介面主要供行銷人員規劃、啟動及衡量其行銷活動。[此頁面](../rn/whats-new.md)列出所有功能。

Campaign 平台依據企業和資料需求所自訂的內容，以及與其他系統之連線，均透過 Campaign 用戶端主控台進行管理。因此，某些設定和功能僅能透過 Campaign 用戶端主控台來存取、建立或管理。其中一些功能將在 Campaign Web 使用者介面的後續更新中提供。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 行銷活動管理 {#campaign-mgt-capabilities}

您可以使用 Campaign Web 使用者介面建立跨管道行銷活動，詳細資訊請參閱[此區段](../campaigns/gs-campaigns.md)。下列功能僅適用於 Campaign 用戶端主控台。您無法在 Campaign Web 使用者介面存取這些功能，但可以從[探索工具選單](user-interface.md#user-interface-explorer)看得到部分功能。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，了解如何使用這些功能。

* **行銷行事曆**。行銷活動行事曆會以全域時間軸顯示所有方案、計劃、行銷活動與傳遞。此功能僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#campaign-calendar){target="_blank"}
* **方案與計劃**。每個行銷活動都屬於某項方案，而該方案則隸屬於某個計劃。在 Campaign Web 使用者介面中，所有行銷活動都會和預設的內建計劃及方案相關聯。您僅能透過用戶端主控台建立和管理計劃及方案。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hant#work-with-plan-and-program){target="_blank"}
* **提供者、預算與成本管理**。您可針對行銷活動內所執行的工作設定參與的服務提供者 (包括成本結構)，並管理每個方案與行銷活動內的預算。 此功能僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=zh-Hant){target="_blank"}
* **分散式行銷** (中央/地方行銷)。Adobe Campaign 提供分散式行銷應用程式，可以讓中央實體 (總公司、行銷部門等) 和地方實體 (銷售點、地區代理商等) 合作實施行銷活動。此功能僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hant){target="_blank"}
* **行銷資源管理** (MRM)、目標、模擬及成本控制。Adobe Campaign 提供行銷資源管理 (MRM) 應用程式，對於相關的任務、預算及行銷資源可進行完整的管理與即時追蹤，讓您透過合作模式控制行銷動作。此功能僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=zh-Hant){target="_blank"}
* **任務管理**。在 MRM 應用程式中，可以從行銷活動控制面板建立、指派、追蹤及監控行銷活動工作。此功能僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=zh-Hant){target="_blank"}

## 通訊管道 {#channels-capabilities}

您可以使用 Campaign Web 使用者介面來建立、設計及傳送&#x200B;**電子郵件**、**簡訊**、**推播**、**直接郵件**，並使用各種專用報告來衡量其影響，詳細資訊請參閱[此區段](../msg/gs-messages.md)。然而，目前&#x200B;**不**&#x200B;適用以下頻道：應用程式內、LINE、呼叫中心/自訂頻道、使用 X (Twitter) 進行社交行銷。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，進一步了解這些頻道。

* **LINE 訊息傳遞**。LINE 是一款應用程式，可免費即時傳送訊息、進行語音通話與視訊通話，適用於所有行動裝置和個人電腦。Adobe Campaign 僅可從用戶端主控台傳送 LINE 訊息。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=zh-Hant){target="_blank"}
* **呼叫中心和自訂管道**。呼叫中心和其他自訂管道可以在您的行銷活動環境中實作。這些管道只能在用戶端主控台中使用。[閱讀 Campaign Classic v7 文件以了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=zh-Hant#other-channels){target="_blank"}
* 搭配 X (Twitter) 進行&#x200B;**社交行銷**。透過 X (Twitter) 張貼訊息和傳送直接訊息，來與客戶互動。此功能隨社交行銷附加元件一併提供，且僅能透過用戶端主控台使用。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=zh-Hant){target="_blank"}

## 登陸頁面和網頁應用程式 {#Webapps-capabilities}

Adobe Campaign 可讓您建立、設計和共用登陸頁面。全新介面中的登陸頁面體驗已完全重新設計。[閱讀此區段](../landing-pages/get-started-lp.md)以探索如何在 Campaign Web 使用者介面中建立、設計和發佈登陸頁面。

因此在 Campaign 用戶端主控台中，您無法編輯、更新或修改在 Web 介面中所建立的登陸頁面，反之亦然。在 Campaign Web 使用者介面中無法使用下列類型的網頁應用程式。不過，其會顯示在登陸頁面清單中。請使用提供的連結來瀏覽 Campaign Classic v7 文件，並深入了解這些網頁應用程式：

* **網頁應用程式**。透過 Adobe Campaign，您可以使用資料庫中預先載入的資料，以及根據連線使用者之權限而調整的內容，建立及發佈動態的互動式網頁應用程式。此功能僅適用於用戶端主控台。[閱讀 Campaign Classic v7 文件了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=zh-Hant){target="_blank"}
* **網路表單**。在 Campaign Web 使用者介面中，可看到用戶端主控台中設計的網頁和登陸頁面，但無法編輯或修改。用戶端主控台網頁頁面設計工具與 Campaign Web 使用者介面提供的登陸頁面設計工具之間，部分選項可能有所差異。[閱讀 Campaign Classic v7 文件以了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hant){target="_blank"}
* **線上意見調查**。您只能從用戶端主控台建立線上意見調查和收集回答。Campaign Web 使用者介面並未提供這項功能。[閱讀 Campaign Classic v7 文件以了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=zh-Hant){target="_blank"}

## 輪廓、測試輪廓和客群 {#profiles-audiences-capabilities}

您在 Campaign 用戶端主控台以及 Campaign Web 使用者介面中皆可以建立、管理及更新輪廓和測試輪廓。在其中一個介面所執行的所有變更，皆可在另一個介面中看到。不過，新的 Campaign Web 使用者介面可能會缺少某些特定的收件者設定和進階參數。

請注意，在新的 Web 使用者介面中，「收件者」一詞已變更為「輪廓」，而「種子地址」現在變成「測試輪廓」。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

在 Campaign 用戶端主控台或 Adobe Experience Platform 中建立的所有客群，都可以在 Campaign Web 使用者介面中使用。

在 Campaign Web 使用者介面中無法使用 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=zh-Hant#import-jobs){target="_blank"}中所述的單次匯入/匯出工作。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html?lang=zh-Hant){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## 內容設計 {#content-capabilities}

Adobe Campaign Web 使用者介面隨附全新的電子郵件設計工具，可讓您透過直覺式的拖放介面，輕鬆建立吸引人、個人化量身打造的電子郵件。無論是從空白顯示窗開始，還是匯入現有內容或者利用現有範本，您可以針對每封電子郵件設計和調整所有內容。[了解更多](../email/edit-content.md)

透過這個全新的使用者介面，您可以管理來自 Adobe Experience Manager 的電子郵件範本同步，以及與 Adobe Experience Manager as a Cloud Service 進行整合。

請注意，目前無法在 Campaign Web 使用者介面中使用下列功能。使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些功能。

* **自訂個人化區塊建立功能**。除了預設的個人化區塊之外，您還可以從用戶端主控台建立自訂區塊。Campaign Web 使用者介面並未提供這項功能。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=zh-Hant#create-custom-personalization-blocks){target="_blank"}
* **自訂表單中的內容**。內容管理模組可讓您建立和管理表單，協助使用者在 Campaign 中建立內容。此功能僅適用於用戶端主控台。[閱讀 Campaign Classic v7 文件以了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=zh-Hant){target="_blank"}
* **電子郵件 AMP**。透過電子郵件 AMP 格式，您可以在訊息中加入 AMP 元件，並使用豐富的可操作內容來改善電子郵件體驗。此功能僅適用於用戶端主控台。[&#x200B; 閱讀 Campaign Classic v7 文件以了解更多資訊](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=zh-Hant){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 類型與類型規則 {#rules-capabilities}

類型是在準備階段執行的一組類型規則，以便輕鬆地將多個篩選規則同時套用於傳遞。藉由控制、篩選及優先處理傳遞內容的傳送，行銷人員可以將所有傳遞的業務實務標準化。

您可以在 Campaign Web 使用者介面中，選取傳遞或傳遞範本的類型規則，詳細資訊請參閱[此區段](../advanced-settings/delivery-settings.md#typology)。不過，您僅可以在 Campaign 用戶端主控台中建立、管理與自訂規則和類型規則。

使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解類型規則：

<!--
* Control rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=zh-Hant){target="_blank"}
-->
* 建立疲勞/壓力規則。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}
<!--
* Filtering rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=zh-Hant){target="_blank"}
* Typology rules management. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=zh-Hant){target="_blank"}
-->
* 模擬行銷活動。[了解更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=zh-Hant){target="_blank"}
<!--
* JavaScript coding for typology rules authoring. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant#use-cases-on-pressure-rules){target="_blank"}
-->

## 工作流程 {#wf-capabilities}

新的 Campaign Web 使用者介面帶來重新設計的工作流程畫布介面，可供您設計和管理流程。新設計的介面中已可使用主要的工作流程活動，而有部分活動將在未來更新中提供。[閱讀此區段](../get-started/guardrails.md)，了解更多關於工作流程功能的資訊，包括護欄和限制。

請注意，下列功能僅可在 Campaign 用戶端主控台中使用：

<!--
* Scripting in workflows
-->

* ETL 活動：匯出、編輯結構描述、資料載入、資料擷取、SQL 程式碼

閱讀[此處](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=zh-Hant){target="_blank"}的 Adobe Campaign v8 (主控台) 工作流程文件，了解更多關於可使用的工作流程活動。

## 產品建議管理 {#offer-capabilities}

您可以在 Adobe Campaign Web 使用者介面中建立的傳遞中傳送產品建議。務必已使用&#x200B;**[!UICONTROL 互動]**&#x200B;模組，在用戶端主控台中建立這些產品建議。產品建議設計、適用性規則和產品建議管理的功能，僅可在 Campaign 用戶端主控台中使用。[了解更多](../msg/offers.md)

閱讀 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hant){target="_blank"}，了解如何管理產品建議目錄。

## 與 Adobe Experience Cloud 解決方案整合 {#exc-capabilities}

新的 Campaign 現代使用者介面簡化了行銷活動的設計與傳遞，並且與其他 Adobe 解決方案 (包括 Adobe Experience Platform 和 Adobe Experience Manager) 的介面保持一致性。

下列整合功能可於 Adobe Campaign 用戶端主控台中使用，但無法在 Campaign Web 使用者介面中使用。使用提供的連結來瀏覽 Campaign v8 (用戶端主控台) 文件，並深入了解這些整合：

* Adobe Analytics 資料使用情況和 KPI 共用。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Experience Cloud 共用客群 (Adobe Audience Manager)。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Target 整合。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=zh-Hant){target="_blank"}
* 與 Adobe Experience Cloud 觸發程序整合。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=zh-Hant){target="_blank"}

## 報告 {#reporting-capabilities}

新的 Campaign Web 使用者介面提供一組適用於所有管道的新報告與 KPI：傳遞報告、行銷活動報告以及全域報告。若要了解詳細資訊，請參閱[本章節](../reporting/gs-reports.md)

部分功能僅能從用戶端主控台取得。瀏覽所提供的 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hant){target="_blank"}連結，了解更多資訊。

* 內建的傳遞能力報告與收件匣呈現。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=zh-Hant){target="_blank"}
* 自訂報告。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=zh-Hant){target="_blank"}
* 描述性分析。[了解更多](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=zh-Hant){target="_blank"}
* 行銷活動分析/多維度資料集報告。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=zh-Hant){target="_blank"}
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
>雖然其中一些活動僅能在用戶端主控台中使用，但有些活動可於 Campaign Web 使用者介面中使用，例如&#x200B;**擴充**、**載入檔案**、**變更資料來源**，或者&#x200B;**變更維度**&#x200B;活動。[了解更多關於 Campaign Web 使用者介面中目標選擇和資料管理活動的資訊](../workflows/activities/about-activities.md#targeting)

### 同盟資料存取設定 {#fda}

Campaign 設定以及與外部系統的連線僅限進階使用者使用，且僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hant){target="_blank"}

## 核准 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="核准管理"
>abstract="核准管理僅能自用戶端控制台進行。 "

Campaign Web 使用者介面不會針對內容、傳遞、工作流程、行銷活動及目標選擇顯示核准管理。這些功能僅適用於用戶端主控台。

若要了解如何管理工作流程核准，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=zh-Hant){target="_blank"}。

若要了解如何管理行銷活動傳遞、內容與目標核准，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=zh-Hant){target="_blank"}。

## 權限 {#permissions-capabilities}

Campaign 使用者僅能使用其 Adobe ID，透過 Adobe 身分管理系統 (IMS) 存取 Campaign Web 使用者介面。授予使用者的權限也適用於 Campaign Web 使用者介面。

相關權限會在 Adobe Admin Console 和 Adobe Campaign 用戶端主控台中定義，詳細資訊請參閱[此區段](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=zh-Hant)。在 Adobe Campaign Web 使用者介面無法針對權限執行任何動作。

## 監視 {#monitoring-capabilities}

Campaign 平台監視功能僅適用於用戶端主控台和 Campaign 控制面板，而不會出現在 Campaign Web 使用者介面中。

瀏覽所提供的 Campaign v8 (用戶端主控台) 文件和控制面板文件連結，了解更多資訊。

* [工作流程監視](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=zh-Hant){target="_blank"}
* [工作流程熱度圖](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=zh-Hant){target="_blank"}
* [效能監視](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=zh-Hant){target="_blank"}
* [傳遞能力監視](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=zh-Hant){target="_blank"}

## 時區管理 {#timezone-management}

Adobe Campaign Web UI會根據使用者網頁瀏覽器&#x200B;**的**&#x200B;當地時區，顯示所有日期和時間值。 在Web UI和使用者端主控台之間比較時間戳記時，此行為可能會導致差異。

請參閱此[頁面](../administration/timezone-management.md)，深入瞭解&#x200B;**Web UI**、**使用者端主控台**&#x200B;與&#x200B;**工作流程執行**&#x200B;時區之間的差異。
