---
title: Campaign Web UI中的護欄和限制
description: Campaign Web UI中的護欄和限制
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 4%

---


# 護欄和限制 {#guardrails-limitations}

使用在Campaign使用者端主控台中建立或修改之元件的Campaign網頁UI時，以下所列護欄和限制適用。

## 工作流程 {#wf-guardrails-limitations}

**活動**

* Web UI中尚未支援的工作流程活動是唯讀的。 您仍然可以執行工作流程、傳送訊息、檢查記錄檔等。 Web UI和使用者端主控台中可用的工作流程活動皆可編輯。

| 主控台 | Web UI |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**畫布**

* 在Web UI中建立新工作流程時，畫布僅支援一個進入點。 不過，如果您在主控台中建立了包含多個進入點的工作流程，

不過，即使您的工作流程是在具有多個進入點的使用者端主控台畫布中建立，也可以在Web UI中編輯。 您仍然可以開啟和編輯



若要嘗試此案例，請從具有多個入口點的使用者端主控台建立工作流程，然後從Web UI開啟該工作流程來檢視結果。



當然，您可以編輯活動，照常啟動及執行工作流程。



**活動定位**

* 節點的位置只有在活動已新增或移除時（並非總是如此），才會重新計算（因此會修改活動的初始位置）。

**未公開選項**

* 不相容的選項不會顯示在Web UI中。

**回圈**

* 網頁UI中尚未提供回圈。 如果您使用主控台建立了包含回圈的工作流程，則無法從Web UI存取它。 畫面會顯示錯誤訊息。

| 主控台 | Web UI |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**調解與擴充**

在Campaign使用者端主控台中， **擴充** 活動可同時執行調解和擴充。 在Campaign Web UI中，尚未提供調解功能。 如果您在主控台活動中設定了調解，則在Web UI中會顯示為不相容活動。

* 如果 **擴充** 主控台中的活動只會執行 **擴充** 活動會顯示在網頁中。
* 如果 **擴充** 主控台中的活動只會執行調解，不相容的活動會顯示。

## 預先定義的篩選 {#filters-guardrails-limitations}

在該版本的產品中，當選取傳送的對象時，或在工作流程中建立對象時，使用者介面中無法使用某些預先定義的篩選器。

此時會顯示特定錯誤訊息。 即使您無法在規則產生器中檢視查詢的圖形表示，也無法編輯篩選，您仍可以使用它，並檢視篩選條件和結果。 您也可以存取SQL查詢以檢查確切的設定。

![](assets/filter-unavailable.png){width="70%" align="left"}

請注意，如果您在Web介面中建立篩選器，並在主控台中使用不支援的屬性來修改篩選器，Web介面中將無法再使用圖形表示。 在任何情況下，您仍可使用篩選器。

以下列出不支援的屬性。

### 不支援的資料型別 {#unsupported-data-type}

在Web介面中顯示篩選器或規則時，不支援使用者端主控台中可用的下列資料型別：

* 日期時間
* 時間
* 時間跨度
* 兩次
* 浮點數

### 不支援的篩選功能 {#unsupported-filtering-capabilities}

若篩選是在使用者端主控台中以複雜的運算式和函式建立，則無法在Web介面中進行編輯。

此外，不支援下列運運算元：

* 數值型別
   * 包含在
   * no in

* 字串型別
   * 大於
   * 小於
   * 大於或等於
   * 小於或等於
   * 按讚
   * 不相似

* 日期型別
   * 在或晚於
   * 在或早於
   * 不等於
   * 是空的
   * 不是空的
   * 包含在
   * 不在
   * 最近

* 1-N連結
   * COUNT， SUM， AVG， MIN， MAX