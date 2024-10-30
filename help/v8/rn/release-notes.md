---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 42%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。

舊版可用的變更和改進專案列於本頁](release-notes-24.md)的[中。

## 2024年10月發行 {#24-10-release}

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
<p>異動訊息（訊息中心）現在可在Campaign網頁使用者介面中使用。 此附加元件專為觸發訊息而設計，這些訊息是從資訊系統觸發的事件所產生，可以是：發票、訂單確認、出貨確認、密碼變更、產品無法使用通知、帳戶對帳單、網站帳戶建立等。</p>
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

* **版本和系統資訊** — 您現在可以存取使用者端主控台和Web使用者介面執行個體版本的詳細資料。 此新區段也會列出環境中安裝的所有內建套件。 [了解更多](../get-started/user-interface.md#user-interface-about)

* **清單** — 您現在可以輕鬆重新排序清單的值。 [了解更多](../get-started/work-with-folders.md)

* **傳遞** — 傳遞變數現在可從個人化欄位存取。 [了解更多](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)