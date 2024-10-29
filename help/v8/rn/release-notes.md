---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

## 10月發行 {#24-10-release}

**發行日期**：2024年10月29日

從10月發行版本開始，將推出下列功能和改善專案。

### 功能

<table>
<thead>
<tr>
<th><strong>外部帳戶</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接透過Adobe Campaign網頁使用者介面設定和管理外部帳戶。 此新功能可讓您輕鬆設定不同型別的外部帳戶，例如退回電子郵件(POP3)或執行個體。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細的文件</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>交易型訊息傳遞功能</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以在Campaign網頁使用者介面中建立和監視異動訊息。 異動訊息是Adobe Campaign中的專門模組，用於處理觸發式訊息。 這些訊息會自動產生，以回應來自資訊系統的事件。 這類事件的常見範例包括按一下按鈕或連結、放棄購買、要求產品可用性警示、建立或修改帳戶等。</p>
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/transactional.md">詳細的文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### 改良功能

* **工作流程活動** — 您現在可以將活動及其所有子節點從工作流程內的轉變移動到另一個轉變。 活動的屬性窗格中有專用的&#x200B;**移動**&#x200B;按鈕可用來執行此動作。 [了解更多](../workflows/orchestrate-activities.md#move)

* **工作流程擴充活動**

   * 現在當您在&#x200B;**擴充**&#x200B;活動中建立新欄位時，可以定義別名與標籤。 [了解更多](../workflows/activities/enrichment.md#collection-settings)
   * 您現在可以在&#x200B;**擴充**&#x200B;活動中為每個設定檔新增優惠。 [了解更多](../workflows/activities/enrichment.md##add-offers)

* **值的分佈** - 當存取個人化的欄位清單時，您現在可以查看每個欄位的值如何分佈。專用的快顯視窗會顯示每個值的數字和百分比。[了解更多](../query/build-query.md#distribution-values-query)


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
<p>完成訊息的製作與量身打造後，請使用Adobe Campaign Web中的AI Assistant Content Accelerator將其提升到新的境界。 這款強大的工具可讓您產生一系列引人入勝的文字、主要標題和吸引人的視覺影像，以最佳化內容的影響力。</p>
<p>透過<a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">我們的即時功能預覽</a>，讓自己沉浸在實作體驗中，以便親身探索並充分了解其功能。</a></p>
<p>如需詳細資訊，請參閱<a href="../email/generative-gs.md">詳細的文件</a>。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>推出日期：9 月 12 日</p>
</td>
</tr>
</tbody>
</table>

## 8月發行 {#24-8-release}

**發行日期**：2024 年 9 月 3 日

以下功能和改良功能將從 8 月版開始提供。

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
