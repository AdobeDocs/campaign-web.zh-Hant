---
audience: end-user
title: 建立和管理優惠方案空間
description: 瞭解如何在Campaign Web中建立、設定、部署和預覽優惠方案空間
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# 建立和管理優惠方案空間 {#offer-space}

**優惠方案空間**&#x200B;定義優惠方案向連絡人公開的位置和方式：它使用哪個管道（電子郵件、直接郵件、簡訊、傳入網路等）、優惠方案可以使用哪些內容欄位，以及如何建立最終呈現。 單一環境可包含多個選件空間 — 每個展示點各一個。

優惠方案空間本身不是管道。 它代表優惠方案在頻道上顯示的特定位置。 相同網頁上的兩個橫幅通常會對應至兩個不同的優惠方案空間。 如需完整的概念模型，請參閱[Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}。

## 建立或修改優惠方案空間{#create-offer-space}

優惠方案空間會儲存在優惠方案環境資料夾下。 若要瀏覽您的平台上可用的優惠方案空間，請開啟&#x200B;**[!UICONTROL Explorer]**，瀏覽至優惠方案環境，然後選取包含優惠方案的子資料夾。

![熒幕擷圖顯示優惠方案空間清單。](assets/offers-space.png){zoomable="yes"}

您可以在此按一下&#x200B;**[!UICONTROL 建立優惠方案空間]**，開啟現有的優惠方案空間或建立新的優惠方案空間。

![顯示優惠方案空間熒幕的熒幕擷圖。](assets/offers-space-1.png){zoomable="yes"}

### 定義屬性 {#properties}

本節可讓您：

* 輸入優惠方案空間的&#x200B;**[!UICONTROL 標籤]**。
* 選取符合說明點（電子郵件、直接郵件、簡訊、網頁等）的&#x200B;**[!UICONTROL 頻道]**。
* 如果此優惠方案空間除了大量傳遞呼叫外，還必須支援對優惠方案引擎的單一（即時、單一優惠）呼叫，請選取&#x200B;**[!UICONTROL 啟用單一模式]**。

### 定義內容欄位 {#content-fields}

內容欄位列出可在選件層級編輯並由演算函式重複使用的屬性。 您在優惠方案空間新增欄位的順序會驅動它們在優惠方案&#x200B;**[!UICONTROL 內容]**&#x200B;區段中顯示的順序。

依預設，每個選件都隨附下列現成可用的內容欄位： **[!UICONTROL 標題]**、**[!UICONTROL 目的地URL]**、**[!UICONTROL 影像URL]**、**[!UICONTROL HTML內容]**&#x200B;以及&#x200B;**[!UICONTROL 文字內容]**。 您可以使用轉譯所需的任何自訂欄位來擴充此清單 — 例如&#x200B;**簡短內容**、**追蹤的URL**&#x200B;或透過結構描述擴充功能新增的任何屬性。

按一下&#x200B;**[!UICONTROL 新增內容欄位]**，然後選取要從選件結構描述公開的屬性，或按一下&#x200B;**[!UICONTROL 編輯運算式]**&#x200B;以定義自訂運算式。

>[!IMPORTANT]
>
>若要讓自訂屬性可從選件&#x200B;**[!UICONTROL Content]**&#x200B;區段編輯，該屬性也必須在[!DNL nms:offer]結構描述的&#x200B;**[!UICONTROL 選件內容]**&#x200B;區段中宣告。 深入瞭解[使用結構描述](../administration/schemas.md)。

### 設定演算函式 {#rendering}

轉譯函式會從內容欄位建立最終優惠方案表示方式。 您可以選擇預設呈現（只輸出原樣內容）或是將欄位與HTML、XML或文字結合的自訂函式。

選取&#x200B;**[!UICONTROL HTML轉譯]**、**[!UICONTROL XML轉譯]**&#x200B;或&#x200B;**[!UICONTROL 文字轉譯]**&#x200B;索引標籤，並啟用&#x200B;**[!UICONTROL 多載轉譯函式]**&#x200B;以啟動它。

使用運算式編輯器來編寫演算函式。 您可以參照[運算式編輯器](../query/expression-editor.md)中定義的內容欄位、選件屬性及任何函式。

>[!NOTE]
>
>如果未定義演算函式，則會使用現成可用的屬性以相同方式傳回選件內容。 只有在優惠方案空間上選取&#x200B;**[!UICONTROL 啟用單一模式]**&#x200B;時，才能使用XML演算函式。

### 設定儲存空間與主張狀態 {#storage}

本節可讓您控制透過此空間產生的主張如何持續存在，以及其狀態在整個生命週期中如何演變：

* **[!UICONTROL 停用主張插入]** — 防止透過此優惠方案空間產生的主張插入主張儲存資料表中。

* 主張上的&#x200B;**[!UICONTROL Status]** — 優惠方案引擎傳回主張時，套用到主張的狀態（通常是傳出傳遞的&#x200B;**[!UICONTROL Presented]**）。

* 接受時&#x200B;**[!UICONTROL 狀態]** — 收件者與優惠方案互動時套用的狀態（通常是&#x200B;**[!UICONTROL 已接受]**）。

可用的狀態值符合使用者端主控台使用的清單。 如需詳細資訊，請參閱主控台檔案中的[Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"}。

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### 設定進階設定 {#advanced}

此區段可讓您定義&#x200B;**[!UICONTROL 目標識別]**。 按一下[新增]****&#x200B;並選取一或多個&#x200B;**[!UICONTROL 收件者]**&#x200B;屬性，或按一下[編輯運算式]**[!UICONTROL 以定義自訂運算式]**。 此設定對於基本優惠方案空間為選用。 如需其完整參考資料和行為，請參閱[Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}。

在&#x200B;**傳入Web頻道**&#x200B;上建立的優惠方案空間，也需要設定網站以顯示優惠方案並呼叫優惠方案引擎。 這項整合是在使用者端主控台中執行 — 請參閱[即時提供優惠方案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"}和[在Campaign v8檔案中設定優惠方案引擎整合](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"}。

## 部署優惠方案空間 {#deploy}

必須先部署優惠方案空間，才能用於傳遞。 儲存您的優惠方案空間，然後按一下[部署]。**** 部署的狀態會反映在優惠方案空間上。

![顯示優惠方案部署的熒幕擷圖。](assets/offers-space-2.png){zoomable="yes"}

## 預覽優惠方案空間 {#preview}

預覽可讓您模擬如何為指定目標選取和呈現選件。

1. 在優惠方案空間中，選取&#x200B;**[!UICONTROL 概觀]**&#x200B;旁的&#x200B;**[!UICONTROL 預覽]**&#x200B;索引標籤。

   ![顯示優惠預覽的熒幕擷圖。](assets/offers-space-3.png){zoomable="yes"}

1. 選取目標設定檔並執行預覽。 相符的選件會連同演算函式產生的表示一併傳回。

>[!NOTE]
>
>如果未傳回任何主張，請檢查優惠方案的適用性規則和空間的設定。

接下來，[在目錄中建立選件](create-offer.md)，並將其指派給此空間。
