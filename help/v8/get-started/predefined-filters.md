---
title: 使用預先定義的篩選器
description: 了解如何在 Adobe Campaign Web 中建立和管理預先定義的篩選器
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: b904870f256ec2eeac9a4e353ea8cb9d854524ee
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 100%

---

# 使用預先定義的篩選器 {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="預先定義的篩選器管理"
>abstract="Campaign Web 使用者介面提供簡單易用的介面，能輕鬆管理和自訂預先定義的篩選器，以符合您的特定需求。建立一次並儲存以供未來使用。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="預先定義的篩選器"
>abstract="Campaign Web 使用者介面提供簡單易用的介面，能輕鬆管理和自訂預先定義的篩選器，以符合您的特定需求。建立一次並儲存以供未來使用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="建立警報條件"
>abstract="您可以從「客戶管理 > 預先定義的篩選器」選單中，建立自己的傳遞篩選器。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-select"
>title="儲存篩選器"
>abstract="選取現有之預先定義的篩選器。預先定義的篩選器是建立並儲存供將來使用的自訂篩選器。在使用查詢建模器進行篩選操作時，這些篩選器可用作捷徑。例如，在篩選資料清單或建立傳遞的客群時可以使用這些篩選器。"

預先定義的篩選器是建立並儲存供將來使用的自訂篩選器。在使用查詢建模器進行篩選操作時，這些篩選器可用作捷徑。例如，在篩選資料清單或建立傳遞的客群時可以使用這些篩選器。

您可以使用現有的內建篩選器來存取特定的資料子集，或建立自己的預先定義的篩選器並將其儲存。

![預先定義的篩選器選單介面](assets/predefined-filters-menu.png){zoomable="yes"}

## 建立預先定義的篩選器 {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="建立預先定義的篩選器"
>abstract="為預先定義的篩選器輸入標籤，然後選取其適用的表格。開啟其他選項以新增說明並將此篩選器設定為我的最愛。然後使用「建立規則」按鈕定義篩選條件。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="建立預先定義的篩選規則"
>abstract="要定義自訂篩選器的篩選條件，請按一下「建立規則」按鈕。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-save"
>title="儲存篩選器"
>abstract="您可以透過此畫面將規則儲存為預先定義的篩選器。您可以建立一個新的預先定義的篩選器，或覆寫現有的篩選器。若要將篩選器另存為最愛，請切換開啟「**[!UICONTROL 最愛篩選器]**」選項。您也可以啟用「**[!UICONTROL 共用篩選器]**」選項，讓其他使用者可以存取該篩選器。"

### 從查詢建模工具建立篩選器 {#create-from-rule-builder}

從[查詢建模工具](../query/query-modeler-overview.md)中儲存某個自訂篩選器以供未來使用。請依照下列步驟操作：

1. 開啟查詢建模工具並定義您的篩選條件。在下方的範例中，篩選出居住在馬德里並且訂閱電子報的收件者。
1. 按一下「**選取或儲存篩選器**」按鈕，然後選取「**另存為篩選器**」。

   ![儲存預先定義的篩選器介面](assets/predefined-filters-save.png){zoomable="yes"}

1. 選取「**建立新篩選器**」，然後輸入該篩選器的名稱和說明。

   ![儲存篩選器詳細資訊介面](assets/predefined-filters-save-filter.png){zoomable="yes"}

   如果需要，您可以將篩選器儲存為最愛。若要了解更多資訊，請參閱[此區段](#fav-filter)。

1. 按一下「**確認**」以儲存您的變更。

您的自訂篩選器現在可以在「**預先定義的篩選器**」清單中取得，並可供所有 Campaign 使用者存取。

### 從篩選器清單中建立篩選器 {#create-filter-from-list}

從左側選單的&#x200B;**預先定義的篩選器**&#x200B;項目中建立篩選器。請依照下列步驟操作：

1. 瀏覽至左側選單中的&#x200B;**預先定義的篩選器**&#x200B;項目。
1. 按一下「**建立篩選器**」按鈕。
1. 輸入篩選器名稱，然後從「**文件類型**」欄位中選取其適用的結構描述。預設結構描述為 `Recipients(nms)`。

1. 定義篩選器的規則。例如，年齡超過 30 歲的輪廓。

   ![年齡超過 30 歲的輪廓的篩選器規則](assets/filter-30+.png){zoomable="yes"}

1. 儲存您的變更。

   ![已儲存新篩選器的介面](assets/new-filter.png){zoomable="yes"}

此篩選器便會新增至預先定義的篩選器清單。如果需要，您可以將篩選器儲存為最愛。若要了解更多資訊，請參閱[此區段](#fav-filter)。

## 將您的篩選器另存為最愛 {#fav-filter}

建立預先定義的篩選器時，啟用&#x200B;**另存為最愛**&#x200B;選項，便能在最愛中看到此預先定義的篩選器。

將篩選器另存為最愛後，所有使用者都可以在篩選器建立清單的&#x200B;**最愛篩選器**&#x200B;區段中使用該篩選器，如下所示：

![最愛篩選器區段](assets/predefined-filters-favorite.png){zoomable="yes"}

## 使用預先定義的篩選器 {#use-predefined-filter}

在定義規則屬性時，可以使用預先定義的篩選器。若要存取預先定義的篩選器，請在查詢建模工具下拉式功能表中，選擇「**選取自訂篩選器**」選項。

針對目前內容存取可用之預先定義的篩選器完整清單，並使用位於下拉式清單&#x200B;**最愛篩選器**&#x200B;區段的捷徑。若要深入了解最愛項目，請參閱[本章節](#fav-filter)。

例如，若要透過預先定義的篩選建立客群，請依照下列步驟操作：

1. 瀏覽至左側選單的「**客群**」項目，然後按一下客群清單左上角的「**建立客群**」按鈕。
1. 輸入客群名稱，然後按一下「**建立客群**」按鈕。
1. 選取「**查詢**」活動，然後從右側窗格按一下「**建立客群**」按鈕。

   ![建立客群介面](assets/build-audience-from-filter.png){zoomable="yes"}

1. 從「**選取或儲存篩選器**」按鈕中，選擇「**選取自訂篩選器**」選項。

   ![「選取自訂篩選器」選項](assets/build-audience-select-custom-filter.png){zoomable="yes"}

1. 瀏覽至要用於建立客群的預先定義的篩選器，選取該篩選器並確認。

   ![預先定義的篩選器清單介面](assets/build-audience-filter-list.png){zoomable="yes"}

1. 檢查此篩選器的規則屬性並進行確認。

   此篩選器現在將用作「**查詢**」活動中的查詢。

   ![使用預先定義的篩選器的查詢活動](assets/build-audience-confirm.png){zoomable="yes"}

1. 儲存您的變更，並按一下「**開始**」按鈕以建立客群，並使其可在客群清單中使用。

## 管理您的預先定義篩選器 {#manage-predefined-filter}

預先定義的篩選器會全部在左側導覽功能表的專用項目中分組。

![預先定義的篩選器清單](assets/list-of-filters.png){zoomable="yes"}

於此清單中，您可以按照以上所述建立新篩選器，並執行下列動作：

* 編輯現有篩選器，並變更其規則和屬性。
* 複製預先定義的篩選器。
* 刪除預先定義的篩選器。

您也可以直接從規則產生器中編輯或刪除預先定義的篩選器。在預先定義的篩選器選擇視窗中，使用「**更多動作**」按鈕。您可以刪除篩選器或加以編輯。您可以變更標籤、新增說明，並將其新增為最愛項目。

![預先定義的篩選器版本](assets/filter-edit.png){zoomable="yes"}

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->