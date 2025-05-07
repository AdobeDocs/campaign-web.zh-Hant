---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: ht
source-wordcount: '689'
ht-degree: 100%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 中列出了先前版本可用的變更和改進。

## 2025 年 4 月版 {#25-4-release}

**發行日期**：2025 年 4 月 29 日


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
<p>呼叫中心管道現在已可在 Campaign Web 使用者介面中使用。此管道是指用於管理和追蹤透過呼叫中心處理的通訊或互動的通訊方法 — 通常是專員撥打給客戶或潛在客戶的電話。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>如需詳細資訊，請參閱<a href="../call-center/gs-call-center.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新的規則產生器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以使用新的規則產生器，協助您在改進的使用者介面中定義複雜的條件。您可以視需要從舊的規則產生器切換到新的規則產生器。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>如需詳細資訊，請參閱<a href="../query/query-modeler-overview.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部帳戶製作</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>身為 Campaign 管理員，您現在可以從 Campaign Web 使用者介面中建立與外部系統的新連線。
您也可以檢視、更新和管理現有的外部帳戶。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改良功能 {#25-4-improvements}

**一般使用者介面改善**

* 現在，使用者介面中可以更清楚地看到結構描述屬性的「欄位說明」、「新增至最愛項目」和「數值分佈」選項。如需詳細資訊，請參閱[詳細說明文件](../get-started/attributes.md)。
* 在介面中，日期和時間現在會根據 Experience League 偏好設定中設定的主要語言來進行顯示。這項改進僅適用於幾種語言。若要查看受支援語言的完整清單，請參閱[詳細說明文件](https://experienceleague.adobe.com/zh-hant/docs/core-services/interface/features/browser-language){target=_blank}。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**電子郵件編輯器**：為了增強 Campaign Web 使用者介面中的可存取性，電子郵件設計工具中現在提供兩個新欄位：它們對應至您電子郵件內容的 `html` 元素中的 `title` 元素和 lang 屬性。除了「預覽文字」欄位之外，您還可以在電子郵件的「內文」區段中定義這些設定。如需詳細資訊，請參閱[詳細說明文件](../email/metadata.md)。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**結構描述**

* 您現在可以從 Campaign Web 使用者介面中編輯清單的臨時結構描述。如需詳細資訊，請參閱[詳細說明文件](../audience/manage-audience.md)。
* 您現在可以在範例畫面中預覽結構描述的自訂欄位。如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。
* 您現在可以使用拖放方式，移動清單中的自訂欄位。如需詳細資訊，請參閱[詳細說明文件](../administration/custom-fields.md#add)。


### 限量開放版本中的新功能 {#25-4-features-la}

>[!AVAILABILITY]
>
>以下功能為限量開放 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。這些功能需要將 Campaign 伺服器升級到 v8.7.4。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hant)」。

* **建立多語言傳遞** - 您現在可以在 Adobe Campaign Web 使用者介面中，使用不同語言傳送多個電子郵件傳遞。多語言傳遞功能可讓您選擇傳遞的預設語言，以及可以傳送傳遞的不同語言。您也可以使用您選擇的語言來預覽這些傳遞。如需詳細資訊，請參閱[詳細說明文件](../email/edit-content.md)。

* **多語言動態報告** - 動態報告現可用於多語言電子郵件傳遞。如需詳細資訊，請參閱[詳細說明文件](../reporting/global-reports.md)。

* **簡訊 REST API 支援 (LA)** - 交易型傳訊 REST API 現在已可用於簡訊管道。當承載中同時存在 email 和 mobilePhone 時，您可以使用「wishedChannel」欄位來指定管道。如果未提供，除非 wishedChannel 明確地要求簡訊，否則預設會使用電子郵件。如需詳細資訊，請參閱[詳細說明文件](https://experienceleague.adobe.com/zh-hant/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}。

