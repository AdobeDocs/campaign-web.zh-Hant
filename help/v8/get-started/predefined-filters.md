---
title: 建立和使用預先定義的篩選器
description: 了解如何在 Adobe Campaign Web UI 中建立和管理預先定義的篩選器
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: ht
source-wordcount: '786'
ht-degree: 100%

---

# 使用預先定義的篩選器 {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="預先定義的篩選器管理"
>abstract="Campaign Web 現在為您提供了人性化介面，可以輕鬆管理和自訂預先定義的篩選器，以滿足您的特定需求。建立一次並儲存以供未來使用。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="預先定義的篩選器"
>abstract="Campaign Web 現在為您提供了人性化介面，可以輕鬆管理和自訂預先定義的篩選器，以滿足您的特定需求。建立一次並儲存以供未來使用。"

預先定義的篩選器就是建立並儲存以供未來使用的自訂篩選器。在使用規則產生器進行任何篩選作業時 (例如篩選資料清單或建立傳遞對象時)，可以將它們當作捷徑使用。

您可以使用現有的內建篩選器來存取資料的特定子集，或建立您自己的預先定義篩選器並加以儲存。

![](assets/predefined-filters-menu.png)

>[!IMPORTANT]
>
>在該版本的產品中，當建立規則、選取傳遞對象或在工作流程中建立對象時，某些預先定義的篩選器在使用者介面中將無法使用。您仍然可以使用它們。[了解更多](guardrails.md#predefined-filters-filters-guardrails-limitations)


## 建立預先定義的篩選器 {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="建立預先定義的篩選器"
>abstract="為預先定義的篩選器輸入標籤，然後選取其適用的表格。開啟其他選項以新增說明並將此篩選器設定為我的最愛。然後使用「建立規則」按鈕定義篩選條件。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="建立預先定義的篩選規則"
>abstract="要定義自訂篩選器的篩選條件，請按一下「建立規則」按鈕。"

### 從規則產生器中建立篩選器 {#create-from-rule-builder}

您可以從規則產生器中儲存某個自訂篩選器以供未來使用。請依照下列步驟操作：

1. 開啟規則產生器並定義您的篩選條件。在下方的範例中，您篩選了居住在馬德里的收件者。
1. 按一下「**選取或儲存篩選器**」按鈕，然後選取「**另存為篩選器**」。

   ![](assets/predefined-filters-save.png)

1. 選取「**建立新篩選器**」，然後輸入該篩選器的名稱和說明。

   ![](assets/predefined-filters-save-filter.png){width="70%" align="left"}

   如果需要，您可以將篩選器儲存為最愛。若要了解詳細資訊，請參閱[本章節](#fav-filter)。

1. 按一下「**確認**」以儲存您的變更。

您的自訂篩選器現在可以在「**預先定義的篩選器**」清單中取得，並可供所有 Campaign 使用者存取。


### 從篩選器清單中建立篩選器 {#create-filter-from-list}


您可以從左側選單的「**預先定義的篩選器**」項目中建立篩選器。若要執行此作業，請依照下列步驟操作：

1. 瀏覽左側選單中的「**預先定義的篩選器**」項目。
1. 按一下「**建立篩選器**」按鈕。
1. 輸入篩選器名稱，然後從「**文件類型**」欄位中選取其適用的結構描述。預設結構描述為 `Recipients(nms)`。

   如果需要，您可以將篩選器儲存為最愛。若要了解詳細資訊，請參閱[本章節](#fav-filter)。

1. 定義篩選器的規則。例如，年齡超過 30 歲的設定檔。

   ![](assets/filter-30+.png)

1. 儲存您的變更。此篩選器便會新增至預先定義的篩選器清單。


## 將您的篩選器另存為最愛 {#fav-filter}

建立預先定義的篩選器時，如果您想要在您的最愛中看到此預先定義的篩選器，您可以啟用「**另存為最愛**」選項。


將篩選器另存為最愛後，所有使用者都可以在篩選器建立清單的「**最愛的篩選器**」區段中使用該篩選器，如下所示：

![](assets/predefined-filters-favorite.png){width="30%" align="left"}


## 使用預先定義的篩選器 {#use-predefined-filter}

在定義規則屬性時，可以使用預先定義的篩選器。若要存取預先定義的篩選器，請在規則產生器下拉式清單中選擇「**選取自訂篩選器**」選項。

然後，您就可以存取可用於目前內容的預先定義篩選器的完整清單。

您也可以使用下拉式清單的「**最愛的篩選器**」區段中可用的篩選器捷徑。若要深入了解最愛項目，請參閱[本章節](#fav-filter)。

例如，若要透過預先定義的篩選器建立對象，請依照下列步驟操作：

1. 瀏覽左側選單中的「**對象**」項目。
1. 按一下「**建立對象**」按鈕。
1. 輸入對象名稱，然後按一下「**建立對象**」按鈕。
1. 選取「**查詢**」活動，然後從右側窗格中按一下「**建立對象**」按鈕。

   ![](assets//build-audience-from-filter.png)

1. 從「**選取或儲存篩選器**」按鈕中，選擇「**選取自訂篩選器**」選項。

   ![](assets/build-audience-select-custom-filter.png)

1. 瀏覽到要用於建立對象的預先定義篩選器，選取它並進行確認。

   ![](assets/build-audience-filter-list.png)

1. 檢查此篩選器的規則屬性並進行確認。

   ![](assets/build-audience-check.png)

   此篩選器現在將用作「**查詢**」活動中的查詢。

   ![](assets/build-audience-confirm.png)

1. 儲存您的變更，並按一下「**開始**」按鈕以建立對象，並使其可在對象清單中使用。

## 管理您的預先定義篩選器 {#manage-predefined-filter}

預先定義的篩選器會全部群組在左側導覽選單的專用項目中。

從此清單中，您可以建立新的篩選器 (如上所述)，並且：

* 編輯現有篩選器，並變更其規則和屬性
* 複製預先定義的篩選器
* 刪除預先定義的篩選器

您可以將預先定義的篩選器加入為最愛，以便在建置規則時快速存取。若要了解詳細資訊，請參閱[本章節](#fav-filter)。

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
