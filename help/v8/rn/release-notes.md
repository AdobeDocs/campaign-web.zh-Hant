---
title: Campaign v8 Web 使用者介面發行說明
description: 探索最新 Campaign Web 使用者介面版本的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 29%

---

# 發行說明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="發行說明"
>abstract="Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，Campaign 發行說明每月更新數次，提供最新功能、改進和修正。 我們建議您定期檢查。"

Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。 因此，這些發行說明每月會更新多次。 請定期進行檢查。

## 2026年7月發行 {#26-7-release}

_2026年7月28日_

### 新功能 {#26-7-features}

<table>
<thead>
<tr>
<th><strong>產品建議管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您現在可以直接從Campaign網頁使用者介面端對端管理優惠方案。 設定優惠方案環境和優惠方案空間、建立優惠方案目錄和類別、建立具有適用規則和優先權的優惠方案，並核准和部署它們以用於您的傳送。 Client Console中仍可使用進階設定。</p>
<p>如需詳細資訊，請參閱<a href="../offers/gs-offer-management.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>品牌設定</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>技術管理員現在可以直接從Campaign Web使用者介面建立及設定品牌，無需使用使用者端主控台。 所有品牌設定，包括身分、子網域和通訊協定、電子郵件標題引數和URL追蹤引數，現在均可在Web UI中使用。</p>
<p>如需詳細資訊，請參閱<a href="../administration/branding/branding-configure.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>電子郵件Designer中的公用資源</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>新增影像至電子郵件時，您現在可以選取<strong>公用資源</strong>。 這可讓您選擇Adobe Campaign執行個體上已可用的影像，例如先前在電子郵件Designer中匯入的檔案，或從使用者端主控台上傳的公共資源。</p>
<p>如需詳細資訊，請參閱<a href="../email/content-components.md#image">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>資料載入(RDBMS)工作流程活動</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>資料載入(RDBMS)</strong>活動現在可在Campaign Web使用者介面中使用。 使用此活動可將資料直接從外部關聯式資料庫載入工作流程。 所擷取的資料可在整個工作流程中使用，並可用於目標市場選擇、擴充或進一步資料處理。</p>
<p>如需詳細資訊，請參閱<a href="../workflows/activities/data-loading-rdbms.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>動態 JavaScript 頁面</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您可以運用動態 JavaScript 頁面 (JSSP) 建置伺服器端頁面，這些頁面在透過 URL 存取時會產生動態內容，例如自訂 API、匯出或網頁應用程式邏輯。 您現在可以直接從Campaign網路使用者介面建立、修改、複製和刪除這些頁面。</p>
<p>如需詳細資訊，請參閱<a href="../administration/dynamic-javascript-pages.md">詳細文件</a>以瞭解詳情。</p>
</td>
</tr>
</tbody>
</table>

### 功能改進 {#26-7-improvements}

* 已對&#x200B;**自訂結構描述組態**&#x200B;進行下列改良：
  * 新的&#x200B;**動作資料**&#x200B;區段可讓您限制自訂結構描述記錄上的可用動作，無論個別資料夾上設定的安全性規則為何。 [閱讀更多](../administration/schemas-action-data.md)
  * 已在&#x200B;**詳細目錄清單組態**&#x200B;區段中新增&#x200B;**自訂篩選器**。 它們可讓您選擇哪些屬性會在清單檢視的篩選窗格中顯示為快速存取欄位。 [閱讀更多](../administration/schemas-custom-filters.md)

* 已對&#x200B;**工作流程**&#x200B;進行下列改進：
  * 刪除工作流程活動現在更加靈活：當活動具有後續活動時，您可以選擇刪除所有活動、僅刪除選定活動，或刪除活動同時將後續活動保留在新分支中。 [閱讀更多](../workflows/orchestrate-activities.md#delete-activity)
  * 您現在可以中斷兩個工作流程活動之間的轉變，而不刪除其中一個。 這可讓您重新組織工作流程圖表，例如暫時保留一組您要保留的活動，而不需要刪除和重新建立活動。 [閱讀更多](../workflows/orchestrate-activities.md#disconnect-transition)
  * 水平與垂直卷軸現在會顯示在工作流程畫布周圍，讓您透過直接拖曳至您要檢視的區域來導覽大型工作流程。 [閱讀更多](../workflows/orchestrate-activities.md)
  * 儲存或啟動/重新啟動工作流程時，如果自您開啟工作流程後，其他使用者修改了Web UI或使用者端主控台中的工作流程，現在會顯示警告。 您可以選擇使用您的變更覆寫其他變更、重新載入工作流程以取得最新版本，或取消。

* **寄件者電子郵件地址**：您現在可以使用&#x200B;**NmsDelivery_senderAddressMask**&#x200B;選項，將傳遞的&#x200B;**寄件者電子郵件**&#x200B;欄位限製為預先定義的地址清單。 [閱讀更多](../administration/options.md#restrict-sender-address)
* **已改善登入錯誤訊息**：當登入嘗試失敗時，Web UI現在會針對幾種情況顯示更具體的錯誤訊息（例如，當使用者未指派安全區域或其IP位址受限制時）。
