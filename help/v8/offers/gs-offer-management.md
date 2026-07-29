---
audience: end-user
title: 開始使用選件管理
description: 瞭解如何在Adobe Campaign網頁版中管理優惠方案
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 763
ht-degree: 3%

---

# 開始使用選件管理 {#gs-offer-management}

此功能可讓您將個人化優惠新增至傳遞，並針對特定內容中的每個設定檔呈現最相關的優惠方案。 優惠方案可以是一或多個產品的簡單通訊訊息或促銷活動。 優惠方案引擎會根據適用性規則和優先順序權重，選取要呈現的最佳主張。

Campaign Web使用者介面可讓您端對端管理優惠方案。 您可以建立及設定優惠方案環境、設計優惠方案空間、建立優惠方案目錄、設定適用性規則、編輯優惠方案內容及發佈優惠方案。

接著會根據&#x200B;**適用性規則**&#x200B;和&#x200B;**優先權權重**，透過傳遞將優惠方案呈現給收件者，以便在特定內容中為每個設定檔選取最佳優惠方案。

>[!NOTE]
>
>Campaign Web使用者介面的重點是最常見的選件管理使用方式。 進階設定仍可在Campaign使用者端主控台中使用。 請參閱[Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hant){target="_blank"}

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## 重要概念 {#concepts}

開始使用選件之前，請先熟悉所涉及的主要物件。

* **優惠方案環境** — 包含優惠方案目錄和相關優惠方案空間的容器。 有兩種型別： **設計**&#x200B;環境（您可在此建立和設定選件）和唯讀&#x200B;**[!UICONTROL 即時]**&#x200B;環境（包含可傳送的已核准和已部署物件）。 [了解更多](offer-environment.md)

* **優惠方案空間** — 定義優惠方案的公開位置和方式（電子郵件、直接郵件、簡訊、傳入網路等）。 此空格會列出可在優惠方案中使用的內容欄位、建立優惠方案表示的轉譯函式，以及驅動主張狀態的儲存設定。 [了解更多](offer-space.md)

* **優惠方案目錄和類別** — 優惠方案會以&#x200B;**類別**&#x200B;和子類別的階層式目錄來組織。 每個類別都可以共用適用性規則、有效日期和&#x200B;**應用程式主題**。 設計環境中會提供預設類別，用於接收所有選件。

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **優惠方案** — 具有自己的適用期間、目標篩選器、權重和內容的個別優惠方案。 在向收件者展示優惠方案之前，會先核准並部署優惠方案。 [了解更多](create-offer.md)

* **優惠方案主張** — 在指定空間（網站上的橫幅、電子郵件、簡訊等）向連絡人呈現優惠方案的結果。 當[在傳遞](../msg/offers.md)中設定選件時，會設定每個傳遞的建議數量。

* **套利** — 優惠方案引擎依優先順序將合格優惠方案排名，以選取要呈現哪些優惠方案的原則。 套利會使用在類別、選件和內容選件上定義的條件。

## 選件管理流程 {#workflow}

Campaign Web UI中典型的端對端流程如下：

1. **檢閱優惠方案環境設定** — 檢查設計/即時對應、資格和體重管理設定。 [了解更多](offer-environment.md)

1. **建立優惠方案空間** — 定義符合您管道的內容欄位、演算函式及進階引數。 [了解更多](offer-space.md)

1. **在目錄中建立優惠方案** — 設定每個優惠方案的適用期間、目標篩選器、權重和內容。 [了解更多](create-offer.md)

1. **核准並部署** — 提交優惠方案以供核准、核准其內容與資格，然後讓部署程式將其發佈到即時環境。 [了解更多](create-offer.md#approve-deploy)

1. **將優惠方案新增至傳遞** — 參考優惠方案空間以及電子郵件、SMS、推播或直接郵件傳遞中的主張。 [了解更多](../msg/offers.md)

## 存取Web UI中的選件 {#access}

可從&#x200B;**[!UICONTROL 優惠]**&#x200B;左側功能表取得優惠。 您可以在此瀏覽目錄、開啟優惠方案以供編輯，以及監控其核准和部署狀態。

![顯示選件功能表的熒幕擷圖。](assets/offers-gs.png){zoomable="yes"}

透過&#x200B;**[!UICONTROL Explorer]**，導覽至對應的資料夾，存取優惠方案環境和優惠方案空間。


## 僅主控台補充 {#console-complements}

部分選件功能尚未在Web使用者介面中公開，仍須從使用者端主控台進行設定：

* **優惠方案模擬** — **模擬**&#x200B;模組可讓您在傳送之前測試優惠方案的分佈。 請參閱[優惠方案模擬](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=zh-Hant#offer-simulation){target="_blank"}。

* **預先定義的篩選器**&#x200B;管理 — 可從任何選件參考的可重複使用的篩選器規則。 請參閱[管理預先定義的篩選器](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}。

* **優惠追蹤** — 設定優惠方案主張的追蹤，以饋送主張歷程記錄。 檢視[追蹤優惠方案主張](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=zh-Hant){target="_blank"}。

* **操作員角色** — 指派優惠方案管理員/傳遞管理員許可權。 請參閱互動模組[&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}的運運算元。

* **互動最佳實務和套利規則**。 請參閱[行銷活動互動最佳實務](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=zh-Hant){target="_blank"}。

* **報告** — Web使用者介面中尚未提供專用的優惠方案和主張報告。