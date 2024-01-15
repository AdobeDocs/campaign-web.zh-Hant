---
audience: end-user
title: 使用Campaign規則產生器建立對象
description: 瞭解如何使用規則產生器
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: bb3df3067c78311fa0ff3b9a52fe9713552fa0cf
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 59%

---

# 使用規則產生器 {#segment-builder}

規則產生器可讓您透過篩選資料庫中包含的資料，定義傳送所定位的母體。 您可以使用它在工作流程中建立對象 **[!UICONTROL 建立對象]** 活動，或直接在建立傳遞以建立一次性對象時。

* [瞭解如何建立受眾](create-audience.md)
* [瞭解如何建立傳遞的一次性對象](one-time-audience.md)

## 調色盤

位於左側的調色盤包含您可以篩選以建立對象的所有元素。您可以使用搜尋列來快速尋找元素。 浮動視窗中包含的圖磚必須移至中央畫布才能設定並加以考慮。

![](assets/segment-builder2.png){width="70%" align="left"}

調色盤分為兩個索引標籤：

* **屬性**：此索引標籤可讓您存取綱要中的所有可用欄位。欄位清單取決於電子郵件範本中定義的目標定位綱要。

* **受眾**：此索引標籤可讓您使用Campaign Classic主控台中或Adobe Experience Platform中定義的其中一個現有對象進行篩選。 瞭解如何在中監視和管理對象 [本節](manage-audience.md)

  >[!NOTE]
  >
  >若要利用 Adobe Experience Platform 對象，您需要設定與目的地的整合。請參閱 [Adobe Experience Platform目標檔案](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hant){target="_blank"}.

## 畫布

畫布是位於中央的區域，您可在其中根據從調色盤新增的元素來設定及結合規則。若要加入新規則，請從調色盤將方磚拖放到畫布。然後畫面會根據要新增的資料類型顯示特定於上下文的選項。

![](assets/segment-builder4.png){width="70%" align="left"}

## 規則屬性窗格

在右側， **規則屬性** 窗格可讓您執行下列動作。

![](assets/segment-builder5.png){width="70%" align="left"}

* **檢視結果：**&#x200B;顯示對象的目標收件者清單。
* **程式碼檢視**：以 SQL 顯示對象的程式碼版本。
* **顯示進階屬性**：如果您想在左側調色盤中檢視完整的屬性清單，請勾選此選項：節點、群組、1-1 連結、1-N 連結。
* **計算**：更新並顯示查詢所定位的設定檔數目。
* **選取或儲存篩選器**：使用預先定義的篩選器來篩選查詢，或將查詢儲存為新篩選器以供日後重複使用。 [瞭解如何使用預先定義的篩選器](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >在該版本的產品中，使用者介面中無法使用某些預先定義的篩選器。 您仍然可以使用它們。[了解更多](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **屬性**：顯示建立之對象的說明。

## 範例

在此範例中，我們建置一個對象，其以所有居住在亞特蘭大或西雅圖且出生於 1980 年之後的客戶為目標。

1. 在調色盤的「**屬性**」索引標籤中，搜尋「**生日**」欄位。將方磚拖放到畫布上。

   ![](assets/segment-builder6.png)

1. 在畫布中，選擇「**之後**」運算子並輸入所需的日期。

   ![](assets/segment-builder7.png)

1. 在調色盤中，搜尋「**城市**」欄位並將其新增到畫布中的第一條規則下方。

   ![](assets/segment-builder8.png)

1. 在欄位中，輸入第一個城市名稱，然後按 Enter 鍵。

   ![](assets/segment-builder9.png)

1. 對第二個城市名稱重複此動作。

   ![](assets/segment-builder10.png)

1. 按一下「**檢視結果**」以顯示符合此查詢的收件者清單和數量。您也可以新增欄以視覺化和查看資料。在我們的範例中，新增「**城巿**」欄，應該會看到亞特蘭大和西雅圖。

   ![](assets/segment-builder11.png)

1. 按一下「**確認**」。