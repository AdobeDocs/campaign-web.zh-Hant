---
audience: end-user
title: 使用區段產生器
description: Campaign v8網頁檔案
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: d5fa13813a22b21fdedd90475ee9258f5003e22d
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 1%

---

# 使用規則產生器定義對象 {#segment-builder}

![](../assets/do-not-localize/badge.png)

本節說明如何在設計新電子郵件時建立對象。 建立的對象只能用於此電子郵件。

規則產生器可讓您透過篩選資料庫中包含的資料來定義訊息所定位的母體。 如果您想要選取現有對象，請參閱此 [節](add-audience.md).

如需規則產生器的詳細資訊，請參閱 [區段服務檔案](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

若要在設計電子郵件時建立新對象，請遵循下列步驟：

1. 從 **對象** 傳送建立助理的區段，按一下 **[!UICONTROL 選取對象]** 按鈕。

   ![](assets/segment-builder0.png)

1. 選擇 **建立自己的**. 規則產生器隨即顯示。

   ![](assets/segment-builder.png)

## 浮動視窗

位於左側的浮動視窗包含您可以篩選的所有元素，以建立您的對象。 浮動視窗中包含的圖磚必須移至中央畫布中，才能進行設定並納入考量。 浮動視窗分為兩個標籤：

* **屬性**:此索引標籤可讓您存取架構中的所有可用欄位。 欄位清單取決於電子郵件範本中定義的定位結構。

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **對象**:此索引標籤可讓您使用Campaign Classic主控台或從Adobe Experience Platform中定義的現有對象之一進行篩選。

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >若要運用Adobe Experience Platform對象，您需要設定與Destinations的整合。 請參閱 [目的地檔案](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hant){target="_blank"}.

您可以使用搜尋列快速尋找元素。

## 畫布

畫布是中央區域，您可以在其中根據從浮動視窗新增的元素來設定和結合規則。 若要新增規則，請從浮動視窗拖曳圖磚，並將其拖放至畫布上。 接著，系統會根據要新增的資料類型，為您顯示內容特定選項。

![](assets/segment-builder4.png){width="70%" align="left"}

## 規則屬性窗格

在右側， **規則屬性** 窗格中，您可以執行以下操作：

![](assets/segment-builder5.png){width="70%" align="left"}

* **查看結果：** 顯示對象鎖定的收件者清單
* **程式碼檢視**:顯示SQL中基於代碼的對象版本。
* **顯示高級屬性**:如果要在左側浮動視窗中檢視屬性的完整清單，請核取此選項：節點、分組、1-1個連結、1-N個連結。
* **屬性**:顯示已建立對象的說明。

## 範例

在此範例中，我們將建立受眾，鎖定居住在亞特蘭大或西雅圖且生於1980年後的所有客戶。

1. 在 **屬性** 頁簽，搜索 **出生日期** 欄位。 將圖磚拖曳至畫布上。

   ![](assets/segment-builder6.png)

1. 在畫布中，選取 **之後** 運算子，然後輸入所需日期。

   ![](assets/segment-builder7.png)

1. 在浮動視窗中，搜尋 **城市** 欄位，並將其新增至第一個規則下方的畫布。

   ![](assets/segment-builder8.png)

1. 在文字欄位中，輸入第一個城市名稱，然後按Enter鍵。

   ![](assets/segment-builder9.png)

1. 對第二個城市名稱重複此操作。

   ![](assets/segment-builder10.png)

1. 按一下 **查看結果** 顯示與查詢匹配的收件人的清單和數目。 您也可以新增欄以視覺化並檢查資料。 在範例中，新增 **城市** 應該看亞特蘭大和西雅圖。

   ![](assets/segment-builder11.png)

1. 按一下 **確認**.

您的對象已定義，且已準備好在您的電子郵件中使用。