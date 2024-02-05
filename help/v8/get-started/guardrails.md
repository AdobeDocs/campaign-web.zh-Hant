---
title: Campaign Web使用者介面的護欄和限制
description: Campaign Web使用者介面的護欄和限制
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 65%

---

# 護欄和限制 {#guardrails-limitations}

在Campaign網頁使用者介面中使用在Campaign使用者端主控台中建立或修改的元件時，以下列出的護欄和限制適用。

## 工作流程 {#wf-guardrails-limitations}

### 活動

Campaign Web使用者介面中尚未支援的工作流程活動是唯讀的，且會顯示為不相容的活動。 您仍然可以執行工作流程、傳送訊息、檢查記錄等。Campaign Web使用者介面和Campaign使用者端主控台中可用的工作流程活動皆可編輯。

| 主控台 | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

Web使用者介面中尚未支援的工作流程活動設定不會顯示。 但是，當執行工作流程時，便會套用這些設定。

| 主控台 | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

在主控台中，「**擴充**」活動可以執行調和和擴充。在Campaign Web使用者介面中，尚未提供調解功能。 如果您已在使用者端主控台中定義 **擴充** 活動，則會在Campaign網頁使用者介面中顯示為不相容的唯讀活動。

| 主控台 | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### 畫布

在Campaign Web使用者介面中建立新工作流程時，畫布僅支援一個進入點。 不過，如果您在主控台中建立了具有多個進入點的工作流程，則可在Campaign Web使用者介面中開啟及編輯該工作流程。

| 主控台 | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

Campaign Web使用者介面中尚未提供回圈。 如果您使用主控台建立包含回圈的工作流程，則無法從Campaign網頁使用者介面存取該工作流程。 將會顯示錯誤訊息。

| 主控台 | Web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

節點的定位會在每次新增或移除活動時重新整理。如果您在主控台中建立工作流程、使用Campaign Web使用者介面修改它，並在主控台中重新開啟它，您可能會注意到一些細微的定位瑕疵。 這對工作流程的流程和任務沒有影響。

| 初始工作流程 | 定位變更 |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## 預先定義的篩選器 {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="此篩選器為唯讀"
>abstract="某些預先定義的篩選器在該產品版本的使用者介面中不可用。 這些篩選器會標記為唯讀。 即使您無法在查詢建模工具中檢視查詢的圖形表示，也無法編輯篩選器，您仍然可以使用它，並可在該畫面的「**屬性**」區段中看到篩選條件。"

在該版本的產品中，當選取傳遞對象或在工作流程中建立對象時，某些預先定義的篩選器在使用者介面中將無法使用。這些篩選器會標記為唯讀。 

將會顯示具體的錯誤訊息。

![](assets/filter-unavailable.png){width="70%" align="left"}

即使您無法在查詢建模工具中檢視查詢的圖形表示，也無法編輯篩選器，您仍然可以使用它，並可在該畫面的「**屬性**」區段中看到篩選條件。

![](assets/rule-edit.png){width="70%" align="left"}

您也可以存取 SQL 查詢來檢查確切的設定。若要執行此作業，請按一下「**程式碼檢視**」按鈕。

![](assets/rule-code-view.png){width="70%" align="left"}

按一下「**計算**」按鈕以檢查有多少項目符合篩選器的條件。

![](assets/rule-calculate.png){width="70%" align="left"}

使用「**檢視結果**」按鈕來顯示這些項目。

![](assets/rule-view-results.png){width="70%" align="left"}

請注意，如果您在 Web 介面中建置篩選器，並在主控台中使用不支援的屬性修改它，就無法再於 Web 介面中使用圖形表示。在任何情況下，您仍然可以使用該篩選器。

不支援的屬性會列示在下方。

### 不支援的資料類型 {#unsupported-data-type}

在 Web 介面中顯示篩選器或規則時，用戶端主控台中可用的下列資料類型不受支援：

* 日期時間
* 時間
* 時間範圍
* 雙精度浮點數
* 浮點數

### 不支援的篩選功能 {#unsupported-filtering-capabilities}

當篩選器是在用戶端主控台中使用複雜的運算式和函數建置時，則無法在 Web 介面中進行編輯。

此外，不支援下列運算子：

* 數值類型
   * 包含在
   * 不在

* 字串類型
   * 大於
   * 小於
   * 大於或等於
   * 小於或等於
   * 類似
   * 不類似

* 日期類型
   * 在或晚於
   * 在或早於
   * 不等於
   * 是空的
   * 不是空的
   * 包含在
   * 不在
   * 在最近

* 1-N 個連結
   * 計數、總和、平均、最小值、最大值
