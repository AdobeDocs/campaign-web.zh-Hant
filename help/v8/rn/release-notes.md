---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 589d78737a498ffe91cb49a6f689f4104b244d0b
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 34%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

舊版可用的變更和改善專案列於[2024](release-notes-24.md)和[2025](release-notes-25.md)。

## 2025年4月發行 {#25-4-release}

**發行日期**： 2025年4月29日


### 新功能 {#25-4-features}

從 4 月版本開始，所有使用者都可以使用以下功能。

<table>
<thead>
<tr>
<th><strong>呼叫中心管道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>客服中心頻道現在可在Campaign網頁使用者介面中使用。 此管道是指用於管理和追蹤透過呼叫中心處理的通訊或互動的通訊方法，通常是由代理對客戶或潛在客戶進行的電話。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>如需詳細資訊，請參閱<a href="../call-center/gs-call-center.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新增規則產生器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>現在有新的規則產生器可用，以協助您在改良的使用者介面中定義複雜條件。 您可以視需要從舊規則產生器切換到新規則產生器。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>如需詳細資訊，請參閱<a href="../query/query-modeler-overview.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部帳戶編寫</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>身為Campaign管理員，您現在可以從Campaign Web使用者介面設定與外部系統的新連線。
您也可以檢視、更新及管理現有的外部帳戶。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改良功能 {#25-4-improvements}

**一般介面改善**

* 結構描述屬性的「欄位」說明、「新增至我的最愛」和「值分佈」選項現在可更加顯示在使用者介面中。 如需詳細資訊，請參閱[詳細說明文件](../get-started/attributes.md)。
* 在介面中，現在會根據Experience League偏好設定中設定的主要語言顯示日期和時間。 這項改善僅適用於數種語言。 若要檢視支援語言的完整清單，請參閱[詳細檔案](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**電子郵件編輯器**：為了增強Campaign Web UI的協助工具，電子郵件Designer現在提供兩個新欄位：它們對應至您電子郵件內容`html`元素中的`title`元素和lang屬性。 除了電子郵件內文區段的「預覽文字」欄位外，您還可以定義這些設定。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**結構描述**

* 您現在可以從Campaign網頁使用者介面編輯清單的暫時綱要。 如需詳細資訊，請參閱[詳細說明文件](../audience/manage-audience.md)。
* 您現在可以在範例畫面中預覽結構的自訂欄位。 如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。
* 您現在可以使用拖放來移動清單中的自訂欄位。 如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。


### 限量開放版本中的新功能 {#25-4-features-la}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。這些環境僅限於將&#x200B;**從Adobe Campaign Standard移轉至Adobe Campaign v8**&#x200B;的客戶，無法部署在任何其他環境中。 這些要求將Campaign伺服器升級至v8.7.4。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hant)」。

* **建立多語言傳遞** — 您現在可以在Adobe Campaign網頁使用者介面中以不同語言傳送多封電子郵件。 多語言傳送功能可讓您選擇傳送的預設語言，以及傳送傳送時所使用的不同語言。 您也可以使用所選的語言預覽這些傳送。 如需詳細資訊，請參閱[詳細說明文件](../email/edit-content.md)。

* **多語言的動態報告** — 多語言電子郵件傳遞現在可使用動態報告。 如需詳細資訊，請參閱[詳細說明文件](../reporting/global-reports.md)。

* **SMS REST API支援(LA)** — 異動訊息REST API現在可用於SMS頻道。 當電子郵件和行動電話都出現在有效負載中時，您可以使用「widedChannel」欄位來指定頻道。 如果未提供，則預設會使用電子郵件，除非widedChannel明確要求SMS。 如需詳細資訊，請參閱[詳細說明文件](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}。

