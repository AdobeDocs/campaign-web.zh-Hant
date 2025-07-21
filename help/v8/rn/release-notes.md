---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 98%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 中列出了先前版本可用的變更和改進。

## 2025 年 7 月更新 {#25-7-updates}

>[!AVAILABILITY]
>
>若要從這些更新中受益，您的伺服器必須至少升級至 8.8.1 版。請參閱用戶端控制台[發行說明](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hant){target="_blank"}。

下列功能先前在可用性受限的狀態下發行，現在已可供所有環境使用 (全面發佈)：

* **建立多語言傳遞** - 您現在可以在 Adobe Campaign Web 使用者介面中，使用不同語言傳送多個電子郵件傳遞。多語言傳遞功能可讓您選擇傳遞的預設語言，以及可以傳送傳遞的不同語言。您也可以使用您選擇的語言來預覽這些傳遞。[閱讀更多](../email/edit-content.md#multilingual-delivery)。

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=zh-Hant){target="_blank"}
-->

* **傳遞提醒** - 傳遞提醒功能是一個警報管理系統，可讓一組使用者自動接收包含其傳遞執行資訊的通知。[閱讀更多](../msg/delivery-alerting.md)

* **登陸頁面改進** - 登陸頁面現已提供下列改進：

   * 現在，您可以在設定服務時參考預設訂閱/取消訂閱登入頁面。設計電子郵件時，如果您定義指向該登陸頁面的連結，則提交登陸頁面表單的使用者會自動訂閱或取消訂閱此服務。[閱讀更多](../audience/manage-services.md#create-service)
   * 登陸頁面設定中的新選項允許匿名訪客存取登陸頁面。如果取消選擇此選項，則只有已識別的使用者才能存取並提交表單。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 登陸頁面設定中的新選項允許在提交登陸頁面時儲存其他內部資料。[閱讀更多](../landing-pages/create-lp.md#create-landing-page)
   * 新選項允許將登陸頁面用於多個服務，使登陸頁面動態化。新增連結到電子郵件時，如果您選擇動態登陸頁面，則可以選取任何服務。如果您選取與特定服務相關的登陸頁面，系統會自動使用該服務 (您無法選取其他服務)。[閱讀更多](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陸頁面現在支援條件內容。[閱讀更多](../landing-pages/lp-content.md)
   * 您可以將登陸頁面連結到服務，並在使用者驗證它後傳送確認訊息。[了解更多](../landing-pages/lp-content.md#lp-message)
   * 您可以新增驗證碼，以保護您的登陸頁面免受機器人程式導致的垃圾訊息和濫用侵害。這對您的客戶來說不會造成干擾，因為它不需要客戶進行任何互動，而且是以與您網站的互動為基礎。[了解更多](../landing-pages/create-lp.md#captcha)

下列功能先前在可用性受限的狀態下發行，現在已&#x200B;**按需**&#x200B;提供：

* **動態報告** - 您現在可以存取動態報告，該報告提供完全可自訂的即時報告來衡量您行銷活動的影響。它新增了對輪廓資料的存取權，除了功能性電子郵件行銷活動資料 (如開啟數和點按數) 外，還可依輪廓維度 (例如，性別、城市和年齡) 進行人口統計分析。動態報告也適用於多語言電子郵件傳遞和交易型訊息。[閱讀更多](../reporting/dynamic-reporting/get-started-reporting.md)

* **集中品牌化** - 您的技術管理員現在可以定義一個或多個品牌，以集中管理影響品牌識別的參數。這包括品牌標誌、登陸頁面存取 URL 之網域或訊息追蹤設定。您可以建立這些品牌，並將其連結至訊息或登陸頁面。 此設定在範本中管理。 品牌化選項適用於所有管道，包括簡訊和直接郵件。[閱讀更多](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >此功能僅適用於新的實作。

除了上方列出的功能外，此版本還隨附一組用戶端控制台中可用的功能：

* [新的SMS傳送聯結器](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=zh-Hant)。 （FDA環境）
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=zh-Hant) （隨選，FDA環境）

請參閱用戶端控制台[發行說明](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hant){target="_blank"}。

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-Hant){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/zh-hant/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->