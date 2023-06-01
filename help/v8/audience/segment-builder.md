---
audience: end-user
title: 使用Campaign規則產生器建立對象
description: 瞭解如何使用規則產生器
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Alpha" type="Positive"
source-git-commit: 1d7c6b94a962e141fb929fa45369326972e5ac04
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 97%

---

# 使用規則產生器定義對象 {#segment-builder}

本章節說明如何在設計新電子郵件時建立對象。建立的對象只能在此電子郵件中使用。

規則產生器可讓您透過篩選資料庫的資料來定義訊息的目標母體。如果要選取現有對象，請參閱本[章節](add-audience.md)。

如需規則產生器的詳細資訊，請參閱[細分服務文件](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html)。

若要在設計電子郵件時建立新對象，請依照以下步驟操作：

1. 從傳遞建立助理的「**對象**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

   ![](assets/segment-builder0.png)

1. 選取「**建立您自己的**」。規則產生器隨即顯示。

   ![](assets/segment-builder.png)

## 調色盤

位於左側的調色盤包含您可以篩選以建立對象的所有元素。調色盤包含的方磚必須移至中央畫布才能進行設定和考慮使用。調色盤分為兩個索引標籤：

* **屬性**：此索引標籤可讓您存取綱要中的所有可用欄位。欄位清單取決於電子郵件範本中定義的目標定位綱要。

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **對象**：此索引標籤可讓您使用在 Campaign Classic 主控台或 Adobe Experience Platform 定義的現有對象進行篩選。

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >若要利用 Adobe Experience Platform 對象，您需要設定與目的地的整合。請參閱[目的地文件](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hant){target="_blank"}。

您可以使用搜尋列快速查找元素。

## 畫布

畫布是位於中央的區域，您可在其中根據從調色盤新增的元素來設定及結合規則。若要加入新規則，請從調色盤將方磚拖放到畫布。然後畫面會根據要新增的資料類型顯示特定於上下文的選項。

![](assets/segment-builder4.png){width="70%" align="left"}

## 規則屬性窗格

在右側的&#x200B;**規則屬性**&#x200B;窗格可讓您執行以下動作：

![](assets/segment-builder5.png){width="70%" align="left"}

* **檢視結果：**&#x200B;顯示對象的目標收件者清單。
* **程式碼檢視**：以 SQL 顯示對象的程式碼版本。
* **顯示進階屬性**：如果您想在左側調色盤中檢視完整的屬性清單，請勾選此選項：節點、群組、1-1 連結、1-N 連結。
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

您的對象已定義並可在您的電子郵件中使用。