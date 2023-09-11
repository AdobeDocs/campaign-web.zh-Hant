---
title: 建立並使用預先定義的篩選器
description: 瞭解如何在Adobe Campaign Web UI中建立和管理預先定義的篩選器
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
source-git-commit: 23a8f5521fd5acd88c0f7ae852ff7e54a081e03a
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 16%

---

# 使用預先定義的篩選器 {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="預先定義的篩選器管理"
>abstract="Campaign Web 現在為您提供了人性化介面，可以輕鬆管理和自訂預先定義的篩選器，以滿足您的特定需求。 建立一次並儲存以供未來使用。"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="預先定義的篩選"
>abstract="Campaign Web 現在為您提供了人性化介面，可以輕鬆管理和自訂預先定義的篩選器，以滿足您的特定需求。 建立一次並儲存以供未來使用。"

預先定義的篩選 是建立和儲存以供日後使用的自訂篩選器。 在使用規則產生器的任何篩選作業期間（例如，篩選資料清單或建立傳送的對象時），都可將這些區段當作捷徑。

您可以使用現有的內建篩選器來存取資料的特定子集，或建立您自己的預先定義篩選器並儲存。

![](assets/predefined-filters-menu.png)


## 建立預先定義的篩選器 {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="建立預先定義的篩選器"
>abstract="為預先定義的篩選器輸入標籤，然後選取其適用的表格。 開啟其他選項以新增說明並將此篩選器設定為我的最愛。 然後使用「建立規則」按鈕定義篩選條件。"


>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="建立預先定義的篩選規則"
>abstract="若要定義自訂篩選的篩選條件，請按一下「建立規則」按鈕。"


若要在規則產生器中儲存自訂篩選器，請遵循下列步驟：

1. 開啟規則產生器並定義篩選條件。 在以下範例中，您會篩選住在馬德里的收件者。
1. 按一下 **選取或儲存篩選器** 按鈕，然後選取 **另存為篩選器**.

   ![](assets/predefined-filters-save.png)

1. 選取 **建立新的篩選器**，並輸入該篩選器的名稱和說明。

   ![](assets/predefined-filters-save-filter.png)

1. （選用）啟用 **另存為最愛** 選項，即可在我的最愛中檢視此預先定義的篩選器。


   篩選器儲存成我的最愛時，此篩選器將可供中的所有使用者使用。 **我的最愛篩選器** 篩選器建立清單的區段，如下所示：

   ![](assets/predefined-filters-favorite.png)


1. 按一下 **確認** 以儲存變更。

您的自訂篩選器現在可在 **預先定義的篩選器** 清單並可供所有Campaign使用者存取。

您也可以從以下專案建立篩選器 **預先定義的篩選器** 左側功能表中的專案。 請依照下列步驟以執行此操作：

1. 瀏覽 **預先定義的篩選器** 左側功能表中的專案。
1. 按一下 **建立篩選器** 按鈕。
1. 輸入篩選器名稱，並從 **檔案型別** 欄位中，選取要套用的結構描述。 預設結構描述為 `Recipients(nms)`.
1. 定義篩選的規則。 例如，30歲以上的設定檔。

   ![](assets/filter-30+.png)

1. 儲存您的變更。篩選器會新增至預先定義的篩選器清單中。

## 使用預先定義的篩選器 {#use-predefined-filter}

定義規則屬性時，可使用預先定義的篩選器。 若要存取預先定義的篩選器，請選擇 **選取自訂篩選器** 選項來建立規則。

然後，您可以存取目前前後關聯可用的完整預先定義篩選器清單。

您也可以使用下列專案所提供的篩選捷徑： **我的最愛篩選器** 區段。

例如，若要從預先定義的篩選器建立對象，請遵循下列步驟：

1. 瀏覽 **受眾** 左側功能表中的專案。
1. 按一下 **建立對象** 按鈕。
1. 輸入對象名稱，然後按一下 **建立對象** 按鈕。
1. 選取 **查詢** 活動，然後在右窗格中按一下 **建立對象** 按鈕。

   ![](assets//build-audience-from-filter.png)

1. 從 **選取或儲存篩選器按鈕**，選擇 **選取自訂篩選器** 選項。

   ![](assets/build-audience-select-custom-filter.png)

1. 瀏覽至用來建立對象的預先定義篩選器，選取並確認。

   ![](assets/build-audience-filter-list.png)

1. 檢查此篩選的規則屬性並確認。

   ![](assets/build-audience-check.png)

   篩選器現在會作為中的查詢 **查詢** 活動。

   ![](assets/build-audience-confirm.png)

1. 儲存變更並按一下 **開始** 按鈕來建立對象，並使其可在對象清單中使用。

## 管理預先定義的篩選器 {#manage-predefined-filter}

預先定義的篩選器都會分組在左側導覽功能表的專用專案中。

從這個清單中，您可以建立如上所述的新篩選器，並且：

* 編輯現有篩選器，並變更其規則和屬性
* 複製預先定義的篩選器
* 刪除預先定義的篩選器

您可以將預先定義的篩選器新增為我的最愛，以便在建立規則時快速存取。 此功能的說明請參閱 [本節](#create-predefined-filter).

## 內建預先定義的篩選器 {#ootb-predefined-filter}

Campaign隨附一組預先定義的篩選器，這些篩選器是從使用者端主控台建立的。 這些篩選器可用來定義您的對象和規則。 不得更改它們。
