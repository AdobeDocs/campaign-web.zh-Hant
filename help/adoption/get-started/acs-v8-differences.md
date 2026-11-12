---
title: Campaign Standard與Campaign v8之間的差異
description: 瞭解從Campaign Standard轉換至Campaign v8時有何變更，以及可在何處尋找詳細資訊
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 25814ce1c70a139c9727b3bfccccd3efe056b441
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 2%
---
# Campaign Standard與Campaign v8之間的差異 {#acs-v8-differences}

Campaign Standard和Campaign v8中的大多數概念相同。 此頁面會收集轉換後對您造成影響的差異，並連結至說明每個差異的頁面。 它可補充[行銷人員](marketers.md)以及[管理員和開發人員](admin-developers.md)的指南。

* 如需術語變更，請參閱[Campaign Standard與Campaign v8](overview.md#experiences)之間的主要差異。
* 若要執行檢查以及轉換後回報的問題，請參閱[轉換後的檢查與疑難排解](post-transition-checks.md)。
* 如需使用者端主控台中才有的功能，請參閱[Campaign Web和Campaign使用者端主控台](../../v8/get-started/capability-matrix.md)。

## 管道和內容 {#channels}

兩個產品中建立和傳送訊息的步驟都類似，如[行銷人員指南](marketers.md)所述。 以下差異與管道可用性、測試傳送、登入頁面及直接郵件工作流程有關。

| 哪些變更 | 了解更多 |
|---|---|
| 應用程式內頻道在Campaign v8中無法使用。 | [應用程式內頻道](marketers.md#acs-gs-marketers-in-app) |
| 若要轉換現有的推播工作流程與傳送，請聯絡您的Adobe Campaign轉換經理。 | [推播通知](marketers.md#acs-gs-marketers-push) |
| 在Campaign Standard中，測試設定檔可標示為&#x200B;**陷阱**&#x200B;以接收最終傳送。 在Campaign v8中，在傳遞的對象設定中新增&#x200B;**陷阱群組**。 | [設陷群組](../../v8/audience/trap-group.md) |
| 在Campaign網頁使用者介面中建立的登入頁面不支援隱藏的輸入欄位或自訂JavaScript。 | [登陸頁面](../../v8/landing-pages/get-started-lp.md) |
| 在Campaign Standard中，直接郵件活動的出站轉變也攜帶了產生的檔案。 在Campaign v8中，僅攜帶目標母體。 若要將檔案傳送至伺服器，請新增&#x200B;**資料擷取**&#x200B;活動，然後新增&#x200B;**檔案傳輸**&#x200B;活動。 | [直接郵件](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## 對象、工作流程和傳遞 {#data-and-workflows}

這些差異會影響從Campaign Standard移轉的對象和工作流程、循環傳遞和&#x200B;**檔案傳輸**&#x200B;活動的某些選項，以及動態報告的範圍。

| 哪些變更 | 了解更多 |
|---|---|
| 對象會在轉換期間轉換。 例如，使用「查詢」活動建立的對象會成為預先定義的篩選器，而檔案型別的對象會成為沒有維度的清單型別對象。 | [管理對象](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standard中執行的工作流程歷史記錄不會移轉。 | [建立工作流程](marketers.md#acs-gs-marketers-wf) |
| 在Campaign Standard中，您可以選取循環電子郵件的彙總期間。 此選項在Campaign v8中無法使用。 | [頻道活動](../../v8/workflows/activities/channels.md) |
| 動態報告涵蓋電子郵件傳送、具有電子郵件傳送的行銷活動以及異動訊息。 | [報告](marketers.md#acs-gs-marketers-reporting) |

## 存取與安全性 {#access}

Campaign Standard安全性群組、角色和組織單位會在轉換期間對應至操作員群組、已命名的許可權和檔案夾許可權。 請檢閱下列幾點，尤其是如果某些使用者的許可權比以前更寬或更窄。

| 哪些變更 | 了解更多 |
|---|---|
| 安全性群組、角色和組織單位會對應至操作員群組、已命名的許可權和檔案夾許可權。 自訂角色不會移轉。 | [使用者存取管理](user-management-acs.md) |
| 具有&#x200B;**資料模型**&#x200B;角色但不具有&#x200B;**管理**&#x200B;角色的使用者可取得&#x200B;**管理**&#x200B;存取權。 | [使用者存取管理](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 在Campaign v8中，指派給具有平行組織單位之安全性群組的使用者可以有更廣泛的存取權。 | [平行組織單位指派](user-management-acs.md#parallel-assignments) |
| 從執行例項存取交易API需要新的產品設定檔。 | [產品設定檔對應](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 隱私權請求可能會在Campaign Standard環境保持作用中期間同時送達Campaign Standard和Campaign v8。 | [隱私權與同意](admin-developers.md#privacy-and-consent) |

## 管理、追蹤和映象頁面 {#admin-tracking}

這些差異會影響轉換前從Campaign Standard傳送的傳遞，以及未轉存至Campaign v8的管理資訊。

| 哪些變更 | 了解更多 |
|---|---|
| 轉換前從Campaign Standard傳送的傳送映象頁面無法使用。 從Campaign v8傳送的傳送映象頁面如常運作。 | [映象頁面](../../v8/email/mirror-page.md) |
| Campaign v8不會擷取在轉換前從Campaign Standard傳送的即時交易傳遞的追蹤資料。 這些訊息的連結仍會重新導向。 | [監視異動訊息](../../v8/transactional-messaging/monitor-transactional.md) |
| 無法使用地理單位。 根據地理單位的存取控制會遺失。 | [存取控制](../../v8/get-started/connect-to-campaign.md#access-control) |

## API和整合 {#apis-and-integrations}

這些差異會影響透過REST API呼叫Campaign的整合功能，以及與其他Adobe解決方案和工具的整合功能。

| 哪些變更 | 了解更多 |
|---|---|
| PKEY值會在移轉後變更。 如果您將PKEY儲存在Campaign之外，請改為遵循API傳回的href。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| 部分已移轉的設定檔欄位（例如時區和`ccpaOptOut`）只會由`profileAndServicesExt/profile` API傳回。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| Campaign v8中不提供Campaign Standard的Dreamweaver和Adobe Experience Platform Data Connector整合。 | [使用Campaign和其他Adobe解決方案](../../v8/integrations/integration.md) |
| Adobe會移轉您的Adobe Analytics和Audience Manager設定。 您必須再次設定觸發器和Adobe Target整合。 | [管理Adobe Campaign整合](admin-developers.md#acs-gs-integrations) |
