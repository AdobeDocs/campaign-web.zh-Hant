---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 8月發行說明 {#24-8-release}

**發行日期**： 2024年9月3日

8月發行版本開始提供下列功能和改善專案。

* **值分佈** — 存取個人化的欄位清單時，您現在可以檢查每個欄位的值分佈方式。 專用快顯視窗會顯示每個值的數目和百分比。 [了解更多](../query/build-query.md#distribution-values-query)

* **SMTP引數** - SMTP設定現在可在電子郵件傳遞設定中使用。 [了解更多](../advanced-settings/delivery-settings.md#smtp)

* **全域變數** — 您現在可以定義全域變數，以定義傳遞的值。 [了解更多](../advanced-settings/delivery-settings.md#variables-delivery)

### 限量開放版本中的新功能 {#acs-24-8}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。
>
>請參閱下列檔案頁面： [Campaign Standard轉換至Campaign v8](../rn/acs-migration.md)和[Campaign Standard使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hant){target="_blank"}。

* **直接郵件的品牌** — 技術管理員現在可以定義一個或多個品牌，以集中影響品牌識別的引數。 這包括品牌標誌、登陸頁面存取 URL 之網域或訊息追蹤設定。您現在可以建立這些品牌，並將其連結至訊息或登入頁面。 此設定在範本中管理。 [了解更多](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **具有登入頁面的訂閱** — 您現在可以將登入頁面連結至服務，並在使用者驗證服務時傳送確認訊息。 [了解更多](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **視覺片段** — 您現在可以封存視覺內容片段。 [了解更多](../content/create-fragment.md#archive)

* **登陸頁面中的驗證碼** — 您現在可以新增驗證碼，以保護登陸頁面免受機器人程式造成的垃圾郵件和濫用。 這對您的客戶來說不會造成干擾，因為它不需要客戶進行任何互動，而且是以與您網站的互動為基礎。[了解更多](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
