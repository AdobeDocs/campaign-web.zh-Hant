---
title: Campaign Web UI中的護欄和限制
description: Campaign Web UI中的護欄和限制
badge: label="Beta"
source-git-commit: 68eb1529f6780682256f4b36bd77d336cf560d21
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 4%

---


# 護欄和限制 {#guardrails-limitations}

使用在Campaign使用者端主控台中建立或修改之元件的Campaign網頁UI時，以下所列護欄和限制適用。

## 工作流程 {#wf-guardrails-limitations}

主控台和Web UI中皆可存取相同的工作流程。 但是，請注意，某些限制適用。

**活動版本**

* 在Web UI中存取主控台工作流程時，您只能修改相容的活動。

**畫布版本**

* 如果主控台工作流程有多個啟動節點/分支或浮動活動，您需要新增啟動活動和分支，以將啟動節點連線到主節點。 您也需要移除浮動活動。

**活動定位**

* 節點的位置只有在活動已新增或移除時（並非總是如此），才會重新計算（因此會修改活動的初始位置）。

**未公開選項**

* 不相容的選項不會顯示在Web UI中。

**回圈**

* 網頁UI中尚未提供回圈。 如果您使用主控台建立了包含回圈的工作流程，將無法在Web UI中存取。 畫面會顯示錯誤訊息。

| 主控台 | Web UI |
| --- | --- |
| ![](assets/limitations-loops-console.png) | ![](assets/limitations-loops-web.png) |

<table>
<tr>
<th>主控台</th>
<th>Web UI</th>
</tr>
<tr>
<td><img src="assets/limitations-loops-console.png"></td>
<td><img src="assets/limitations-loops-web.png"></td>
</tr>
</table>

**調解與擴充**

在Campaign使用者端主控台中， **擴充** 活動可同時執行調解和擴充。 在Campaign Web UI中，尚未提供調解功能。 如果您在主控台活動中設定了調解，則在Web UI中會顯示為不相容活動。

* 如果 **擴充** 主控台中的活動只會執行 **擴充** 活動會顯示在網頁中。
* 如果 **擴充** 主控台中的活動只會執行調解，不相容的活動會顯示。

## 預先定義的篩選 {#filters-guardrails-limitations}

選取傳送的對象時，或是在工作流程中建立對象時，該版本產品的使用者介面中無法使用某些預先定義的篩選器。

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