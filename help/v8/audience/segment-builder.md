---
audience: end-user
title: 使用Campaign規則產生器建立對象
description: 瞭解如何使用規則產生器
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 24%

---

# 使用規則產生器 {#segment-builder}

規則產生器可讓您透過篩選資料庫中包含的資料，定義傳送所定位的母體。 透過使用&#x200B;**[!UICONTROL 建立對象]**&#x200B;活動的工作流程，或直接在建立傳遞以建立一次性對象時，使用此工具來建立對象。

* [瞭解如何建立和儲存對象](create-audience.md)
* [瞭解如何建立傳遞的一次性對象](one-time-audience.md)

## 調色盤

浮動視窗位於左側，包含您可篩選以建立對象的所有元素。 使用搜尋列快速尋找元素。 將浮動視窗中包含的圖磚移至中央畫布以進行設定並加以考慮。

![顯示篩選選項和索引標籤的調色盤介面](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

調色盤分為兩個索引標籤：

* **屬性**：此索引標籤提供結構描述中所有可用欄位的存取權。 欄位清單取決於電子郵件範本中定義的目標定位結構描述。

* **對象**：此索引標籤可讓您使用Campaign Classic主控台中或Adobe Experience Platform中定義的其中一個現有對象進行篩選。 在[本節](manage-audience.md)中瞭解如何監視和管理對象。

  >[!NOTE]
  >
  >若要使用Adobe Experience Platform受眾，請設定與目的地的整合。 請參閱[Adobe Experience Platform目的地檔案](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hant){target="_blank"}。

## 畫布

畫布是中央區域，您可以在其中根據從浮動視窗新增的元素設定及合併規則。 若要加入新規則，請從調色盤將方磚拖放到畫布。上下文特定選項是根據要新增的資料型別而顯示的。

![顯示規則組態選項的畫布介面](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## 規則屬性窗格

在右側，**規則屬性**&#x200B;窗格可讓您執行下列動作。

![顯示可用動作的規則屬性窗格](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **檢視結果：**&#x200B;顯示對象定位的設定檔清單。
* **程式碼檢視**：顯示SQL中對象的程式碼型版本。
* **顯示進階屬性**：核取此選項以檢視左側浮動視窗中的完整屬性清單，包括節點、群組、1-1連結和1-N連結。
* **計算**：更新並顯示查詢所定位的設定檔數目。
* **選取或儲存篩選器**：使用預先定義的篩選器來篩選查詢，或將查詢儲存為新的篩選器，以供日後重複使用。 [瞭解如何使用預先定義的篩選器](../get-started/predefined-filters.md)。

  >[!IMPORTANT]
  >
  >在此版本的產品中，使用者介面中無法使用某些預先定義的篩選器。 您仍然可以使用它們。[了解更多](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)。

* **屬性**：顯示已建立對象的說明。

## 範例

在此範例中，建立受眾的目標是居住亞特蘭大或西雅圖且出生於1980年之後的所有客戶。

1. 在調色盤的「**屬性**」索引標籤中，搜尋「**生日**」欄位。將方磚拖放到畫布上。

   ![新增出生日期欄位至畫布](assets/segment-builder6.png){zoomable="yes"}

1. 在畫布中，選擇「**之後**」運算子並輸入所需的日期。

   ![設定「出生日期」欄位的After運運算元](assets/segment-builder7.png){zoomable="yes"}

1. 在調色盤中，搜尋「**城市**」欄位並將其新增到畫布中的第一條規則下方。

   ![正在新增城市欄位至畫布](assets/segment-builder8.png){zoomable="yes"}

1. 在欄位中，輸入第一個城市名稱，然後按 Enter 鍵。

   ![在「城市」欄位中輸入第一個城市名稱](assets/segment-builder9.png){zoomable="yes"}

1. 對第二個城市名稱重複此動作。

   ![在「城市」欄位中輸入第二個城市名稱](assets/segment-builder10.png){zoomable="yes"}

1. 按一下「**檢視結果**」以顯示符合此查詢的收件者清單和數量。新增欄以視覺化及檢查資料。 在此範例中，新增&#x200B;**City**&#x200B;欄以檢視亞特蘭大和西雅圖。

   ![檢視City資料行新增的結果](assets/segment-builder11.png){zoomable="yes"}

1. 按一下「**確認**」。