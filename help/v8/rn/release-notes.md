---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

[此頁面](release-notes-24.md)列出先前版本可用的變更和改良功能。

## 2024 年 10 月發行版本 {#24-10-release}

**發行日期**：2024 年 10 月 29 日

以下功能和改良功能將從 10 月版開始提供。

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
<p>您現在可以直接透過 Adobe Campaign Web 使用者介面設定和管理外部帳戶。這項新功能可讓您輕鬆設定不同類型的外部帳戶，例如退回電子郵件 (POP3) 或執行執行個體。</p>
<p>如需詳細資訊，請參閱<a href="../administration/external-account.md">詳細說明文件</a>。</p>
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
<p>交易型訊息傳遞功能 (訊息中心) 目前可在 Campaign Web 使用者介面中使用。此附加元件專為觸發訊息而設計，訊息由資訊系統觸發的事件所產生，可以是：發票、訂單確認、出貨確認、密碼變更、產品無法提供的通知、帳戶對帳單、網站帳戶建立等。</p>
<p>如需詳細資訊，請參閱<a href="../transactional-messaging/transactional.md">詳細說明文件</a>。</p>
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

* **工作流程活動** - 您現在可以在工作流程中，將活動及其所有子節點從一個轉變移到另一個轉變。在活動的屬性窗格中，有一個專用的&#x200B;**移動**&#x200B;按鈕可執行此操作。[了解更多](../workflows/orchestrate-activities.md#move)

* **工作流程擴充活動**

   * 現在，您可以在&#x200B;**擴充**&#x200B;活動中建立新欄位時，定義別名和標籤。[了解更多](../workflows/activities/enrichment.md#collection-settings)
   * 您現在可以在&#x200B;**擴充**&#x200B;活動中，為每個客戶輪廓新增優惠方案。[了解更多](../workflows/activities/enrichment.md##add-offers)

* **值的分佈** - 當存取個人化的欄位清單時，您現在可以查看每個欄位的值如何分佈。專用的快顯視窗會顯示每個值的數字和百分比。[了解更多](../query/build-query.md#distribution-values-query)

* **版本和系統資訊** - 您現在可以透過用戶端控制台和 Web 使用者介面，存取執行個體版本的詳細資訊。此新區段也會列出您環境中安裝的所有內建套件。[了解更多](../get-started/user-interface.md#user-interface-about)

* **清單** - 您現在可以輕鬆重新排序清單的值。[了解更多](../get-started/work-with-folders.md)

* **傳送** - 現在可以從個人化欄位存取傳送變數。[了解更多](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)