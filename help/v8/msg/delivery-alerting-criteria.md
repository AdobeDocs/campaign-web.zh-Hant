---
audience: end-user
title: 傳遞警報
description: 瞭解如何使用傳送警報。
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 7%

---

# 傳遞警報條件 {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="傳遞警報條件儀表板"
>abstract="Campaign Web使用者介面提供預先定義的警示准則（輸送量低的傳送、準備失敗的傳送……），您可以將這些准則新增至您的儀表板。 您也可以根據自己的需求建立條件。"

Campaign Web使用者介面提供預先定義的警示准則（輸送量低的傳送、準備失敗的傳送……），您可以將這些准則新增至您的儀表板。 您也可以根據自己的需求建立條件。

警報條件可從 **傳遞警報** 功能表，位於左側導覽窗格的 **條件** 標籤。

![](assets/alerting-criteria-list.png)

## 預先定義的警示准則 {#ootb-criteria}

Campaign Web使用者介面中提供預先定義的警示准則。 這些條件涵蓋一系列案例，如下所示：

* **傳遞失敗**：在定義的範圍內排程的任何傳遞，具有錯誤狀態。
* **具有準備的傳遞失敗**：在定義的範圍內修改的任何傳送，其準備步驟（目標計算和內容產生）已失敗。
* **軟退信的錯誤率很低的傳遞**：在定義的範圍內排程的任何傳遞，其狀態至少為「進行中」，軟跳出錯誤率大於定義的百分比。
* **硬退信的錯誤率很低的傳遞**：在定義的範圍內排程的任何傳遞，其狀態至少為「進行中」，且硬跳出錯誤率大於定義的百分比。
* **長時間開始擱置的傳遞**：在定義的範圍內排程的任何傳遞，其「開始擱置」狀態超過定義的持續時間，「開始擱置」狀態表示系統尚未考慮訊息。
* **低輸送量的傳遞**：任何已開始的傳送時間超過定義的持續時間，且已處理訊息的百分比低於定義的，而輸送量低於定義的值。
* **傳遞進行中**：在定義的範圍內排程的任何傳遞，其狀態為「進行中」。

>[!NOTE]
>
>預設值會套用至上述條件的所有引數。 這些值可在以下位置自訂： **條件引數** 傳送警示儀表板中使用儀表板的區段。 [瞭解如何使用儀表板](../msg/delivery-alerting-dashboards.md)

## 建立警報標準 {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="建立傳遞警報條件"
>abstract="除了Adobe Campaign提供的預先定義警示條件之外，您也可以根據自己的需求建立條件。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="要在警報中新增的指標"
>abstract="選取要顯示為電子郵件警示「詳細資訊」區段欄的指標。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="警報類型"
>abstract="指定 **警示型別** 對於條件，表示標籤和顏色會顯示在警示的「摘要」區段中的傳送條件旁邊。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="條件頻率"
>abstract="控制每個符合條件的傳遞每天的警報頻率。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="建立警報標準"
>abstract="若要建立您自己的傳遞篩選器，請在 Campaign v8 主控台中，透「**管理**」>「**設定**」>「**預先定義的篩選器**」節點建立新的預先定義篩選器。"

若要建立新條件，請遵循下列步驟：

1. 導覽至 **傳遞警報** 功能表並選取 **條件** 標籤。
1. 按一下 **建立傳遞警報條件** 按鈕。
1. 提供條件的標籤。 內部名稱會自動填入且為唯讀。
1. 此 **依此條件套用的傳遞篩選器** 可讓您套用預先定義的篩選條件，以縮小條件的範圍。

   在以下範例中， **傳遞進行中(critInProgressDeliveries)** 已選取篩選器，表示該條件只會考慮狀態為「進行中」的傳送。

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >如果沒有任何預先定義的篩選器符合您的需求，您可以聯絡您的管理員以建立自己的篩選器。  如需如何在Campaign主控台中建立預先定義篩選器的詳細資訊，請參閱 [Adobe Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >這項作業只能由進階使用者執行。

1. 在 **要新增警示的指標** 區段，選擇要顯示為電子郵件警示「詳細資訊」區段欄的指標。

1. 指定 **警示型別** 對於條件，表示標籤和顏色會顯示在警示的「摘要」區段中的傳送條件旁邊。

1. 此 **條件頻率** 區段可讓您針對符合條件的每個傳送，控制每天的警報頻率：

   * **此傳遞標準將在每個通知中重複**：在當天的每個電子郵件警報中顯示符合條件的傳遞。
   * **此傳送條件只會在當天第一次發生時傳送**：僅顯示符合當天第一個報表條件的傳遞，不會在後續電子郵件警報中重複。
