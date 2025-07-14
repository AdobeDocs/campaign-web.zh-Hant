---
audience: end-user
title: 從 Campaign Standard 轉換到 Adobe Campaign Web
description: 探索 Campaign Web 使用者介面
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: ht
source-wordcount: '587'
ht-degree: 100%

---

# Campaign Standard 轉換到 Campaign v8 {#acs-to-ac}

Adobe Campaign Standard 使用者現在可以轉換到 Adobe Campaign Managed Cloud Services v8。轉換後可享有數項優勢：

* **強大的 IT 基礎結構**：Managed Cloud Services v8 提供更為強大的 IT 基礎結構，確保提升行銷活動的效能、可靠性和擴充性。
* **加強支援**：Managed Cloud Services 團隊提供一流的協助，確保您能順暢轉換並持續監視平台。支援包括疑難排解和主動維護。
* **與 Adobe Experience Platform 整合**：Managed Cloud Services v8 與 Adobe Experience Platform 順暢連結，讓使用者能夠充分利用其資料，並在多個管道傳遞具影響力的個人化行銷活動。
* **一致的使用者介面和體驗**：轉換到 Managed Cloud Services v8 不會中斷工作流程。使用者能繼續享受熟悉的介面和體驗，將團隊的學習曲線降至最低。

**若您是從 Campaign Standard 轉換到 Campaign v8 的使用者，請閱讀[此文件](../../adoption/home.md)了解如何開始。**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 主要功能 {#key-features}

Campaign v8 使用者可以存取新的 Campaign Web 介面以及 v8 主控台。兩個環境之間的資料和設定會同步處理。用戶端主控台中可使用的所有資料和設定，在 Campaign Web 使用者介面中皆能看見，可從探索工具左側導覽存取。[了解更多](../get-started/user-interface.md#user-interface-explorer)

Campaign Web 使用者介面專為行銷人員所設計，能用於輕鬆建置和協調其行銷活動。Campaign v8 Web 使用者介面的主要功能包括：

* **現代化、易用且統一的體驗**。[了解更多](../get-started/connect-to-campaign.md)。
* **全新的強大功能和順暢流程**。[了解更多](../get-started/user-interface.md)。
* **易用的簡化版查詢建模工具**。[了解更多](../query/query-modeler-overview.md)。
* **內建的跨管道行銷活動管理功能**。[了解更多](../msg/gs-messages.md)。
* **重新設計的行銷活動工作流程活動**。[了解更多](../workflows/gs-workflows.md)。
* **輕鬆建立和管理輪廓**。[了解更多](../audience/about-recipients.md)。
* **預先定義的篩選器**。[了解更多](../get-started/predefined-filters.md)。
* **用於電子郵件設計的 HTML 轉換器**。[了解更多](../email/existing-content.md)。
* **提供產品建議的簡訊**。[了解更多](../msg/offers.md)。

Campaign 用戶端主控台專為管理員和開發人員所設計，能用於設定及自訂其環境。關於 Campaign 用戶端主控台中可使用之主要功能的詳細資訊，請參閱[此文件](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/new/whats-new){target="_blank"}。

>[!NOTE]
>
>如需了解更多關於 Campaign Web 使用者介面和 Campaign 用戶端主控台所支援及不支援的功能和互通性資訊，請參閱[此頁面](../get-started/capability-matrix.md)。

## 術語 {#terminology}

Campaign v8 和 Campaign Standard 之間大多數概念相似。但是，在術語方面有些不同之處。例如：

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## 特定功能 {#new-features}

為確保能順暢轉換到 Campaign v8，Campaign Standard 的主要功能已新增至 Campaign v8 中。這些功能在[此文件](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hant){target=&quot;_blank}中有詳細介紹，並且僅適用於從 Campaign Standard 轉換的使用者。

* **動態報告**：動態報告提供可自訂的即時報告，方便衡量行銷活動的影響。動態報告亦可以存取輪廓資料，以便按照維度 (例如性別、城市和年齡) 以及功能性電子郵件行銷活動資料 (例如開啟和點按次數)，進行人口統計分析。[了解更多](../reporting/dynamic-reporting/get-started-reporting.md)。

* **集中品牌化**：各家公司可以利用 Adobe Campaign 定義品牌視覺化與技術準則。使用者可以向客戶呈現一致的品牌形象，包含標誌以及電子郵件發送者、URL 或網域等技術層面。[了解更多](../administration/branding/branding-gs.md)。

* **REST API**：從 Campaign Standard 移轉的使用者，可以透過 REST API 為 Adobe Campaign 建立整合，以及將 Adobe Campaign 與其他技術進行連結來建置生態系統。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=zh-Hant){target="_blank"}。

* **登陸頁面**：Campaign v8 登陸頁面已有改進，確保功能與 Campaign Standard 相同。請參閱[發行說明](../rn/release-notes.md#new-24-4)和登陸頁面[文件](../landing-pages/get-started-lp.md)以了解更多資訊。

* **視覺片段**：視覺片段為在一或多個電子郵件傳遞或者內容範本中參照的可重複使用視覺元件。修改片段會更新使用該片段的所有內容。透過改進過的設計流程，行銷使用者可以利用這項功能預先建置多個自訂的內容區塊，以便快速組裝訊息內容。[了解更多](../content/use-visual-fragments.md)。

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->