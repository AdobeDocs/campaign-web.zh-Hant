---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: aea828da825a416dece6c4bee1da6d4e570e4e48
workflow-type: ht
source-wordcount: '481'
ht-degree: 100%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 9 月更新 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI 助理內容加速器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>在精心製作並自訂您的訊息後，請利用 Adobe Campaign Web 中的 AI 助理將訊息提升到新的水準，以實現內容加速。這款強大的工具可讓您產生一系列引人入勝的文字、主要標題和吸引人的視覺影像，以最佳化內容的影響力。</p>
<p>透過<a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">我們的即時功能預覽</a>，讓自己沉浸在實作體驗中，以便親身探索並充分了解其功能。</a></p>
<p>如需詳細資訊，請參閱<a href="../email/generative-gs.md">詳細的文件</a>。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>推出日期：9 月 12 日</p>
</td>
</tr>
</tbody>
</table>

## 8 月發行說明 {#24-8-release}

**發行日期**：2024 年 9 月 3 日

以下功能和改良功能將從 8 月版開始提供。

* **值的分佈** - 當存取個人化的欄位清單時，您現在可以查看每個欄位的值如何分佈。專用的快顯視窗會顯示每個值的數字和百分比。[了解更多](../query/build-query.md#distribution-values-query)

* **SMTP 參數** - 現在可以在電子郵件傳遞設定中找到 SMTP 設定。[了解更多](../advanced-settings/delivery-settings.md#smtp)

* **全域變數** - 現在您可以定義全域變數來設定傳遞的值。[了解更多](../advanced-settings/delivery-settings.md#variables-delivery)

### 限量開放版本中的新功能 {#acs-24-8}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hant){target="_blank"}」。

* **直接郵件的品牌化** - 技術管理員現在可以定義一或多個品牌，以集中管理影響品牌識別的參數。這包括品牌標誌、登陸頁面存取 URL 的網域，或訊息追蹤設定。您現在可以建立這些品牌，並將其連結到訊息或登陸頁面。此設定在範本中管理。 [了解更多](https://experienceleague.adobe.com/zh-hant/docs/experience-cloud/campaign/branding/branding-assign)

* **訂閱與登陸頁面** - 現在您可以將登陸頁面連結到服務，並在使用者驗證後發送確認訊息。[了解更多](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **視覺片段** - 您現在可以封存視覺內容片段。[了解更多](../content/create-fragment.md#archive)

* **登陸頁面中的驗證碼** - 現在您可以新增驗證碼以保護您的登陸頁面，避免受機器人程式導致的垃圾訊息和濫用侵害。這對您的客戶來說不會造成干擾，因為它不需要客戶進行任何互動，而且是以與您網站的互動為基礎。[了解更多](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
