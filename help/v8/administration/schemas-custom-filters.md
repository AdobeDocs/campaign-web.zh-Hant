---
title: 新增自訂篩選器
description: 瞭解如何在清單檢視的篩選器窗格中將自訂篩選器新增為快速存取欄位。
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# 新增自訂篩選器 {#custom-filters}

**[!UICONTROL 詳細目錄清單組態]** > **[!UICONTROL 自訂篩選器]**&#x200B;區段可讓您選擇哪些屬性會在結構描述清單檢視的[篩選器窗格](../query/filter.md)中，於&#x200B;**[!UICONTROL 進階篩選器]**&#x200B;規則產生器上方，顯示為快速存取欄位。

如需有關熒幕定義畫面以及如何存取畫面的詳細資訊，請參閱[存取畫面定義](schemas-browse-access.md#screen-def)區段。

## 新增自訂篩選器 {#add}

1. 瀏覽至&#x200B;**[!UICONTROL 結構描述]**&#x200B;功能表，並使用篩選器找到可編輯的結構描述。

1. 選取清單中的結構描述名稱以開啟它，然後按一下結構描述詳細資料檢視中的&#x200B;**[!UICONTROL 熒幕版本]**&#x200B;按鈕以存取熒幕定義。

1. 移至&#x200B;**[!UICONTROL 詳細目錄清單組態]**&#x200B;區段，然後按一下&#x200B;**[!UICONTROL 自訂篩選器]**&#x200B;表格上方的省略符號圖示，然後選擇&#x200B;**[!UICONTROL 選取屬性]**。

   ![自訂篩選器選擇](assets/schemas-custom-filters1.png)

1. 選取一或多個屬性並確認。

   您可以選擇：

   * 結構描述的直接屬性，例如程式碼或類別。
   * 連結屬性，例如連結至產品的品牌。 在此情況下，篩選器會使用僅限於連結結構描述的搜尋選擇器。
   * 連結的子屬性，例如連結資料夾的全名或連結收件者的電子郵件。

   ![屬性選擇器顯示直接屬性和連結子屬性](assets/schemas-custom-filters2.png)

1. 按一下「**[!UICONTROL 儲存]**」。 您可以使用上下箭頭或拖曳自訂篩選器來重新排序自訂篩選器，並使用其列中的垃圾桶圖示來移除篩選器。

1. 瀏覽至此結構描述的記錄清單，並開啟篩選器窗格。 您選取的屬性會顯示為&#x200B;**[!UICONTROL 自訂篩選器]**，在&#x200B;**[!UICONTROL 進階篩選器]**&#x200B;規則產生器上方。

   ![篩選窗格中顯示的自訂篩選器](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >根據日期或日期和時間屬性的自訂篩選器會顯示為日期範圍選取器。

1. 在其中一個自訂篩選條件中輸入或選取值，以調整清單。

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->