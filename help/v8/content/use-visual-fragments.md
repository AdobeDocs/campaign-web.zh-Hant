---
audience: end-user
title: 在您的電子郵件中新增視覺片段
description: 瞭解如何將視覺化片段新增至您的電子郵件
badge: label="有限可用性"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 13%

---

# 在您的電子郵件中新增視覺片段 {#use-visual-fragments}

>[!AVAILABILITY]
>
>此功能需要更新Campaign v8.6.4。進一步瞭解[Campaign v8使用者端主控台發行說明](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/releases/release-notes)。

在Campaign網頁介面中，**視覺片段**&#x200B;是預先定義的視覺化區塊，您可以在多個[電子郵件傳遞](../email/get-started-email-designer.md)或[內容範本](../email/use-email-templates.md)中重複使用。 在[本節](fragments.md)中瞭解如何建立和管理內容片段。

![使用中的視覺化片段的視覺化表示](assets/do-not-localize/fragments.gif)

## 使用視覺片段 {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="片段選項"
>abstract="此窗格提供與所選片段相關的選項。它可讓您選擇要顯示片段的裝置，並打開該片段的內容。可使用「**[!UICONTROL 樣式]**」標籤進一步自訂您的片段。您還可以打破與原始視覺片段的繼承。"

<!-- pas vu dans l'UI-->

若要在電子郵件內容中插入視覺化片段，請依照下列步驟操作：

1. 使用[電子郵件Designer](../email/get-started-email-designer.md)開啟任何電子郵件或範本內容。

1. 從左側邊欄選取&#x200B;**[!UICONTROL 片段]**&#x200B;圖示。

   ![在電子郵件Designer介面中顯示片段圖示的熒幕擷圖](assets/fragments-in-designer.png)

1. 將會顯示在目前沙箱上建立的所有視覺化片段清單。 您可以：

   * 輸入特定片段的標籤以搜尋該片段。
   * 以遞增或遞減順序排序片段。
   * 變更片段的顯示方式（卡片或清單檢視）。

   >[!NOTE]
   >
   >片段會依建立日期排序。 最近新增的片段會先出現在清單中。

   如果您在編輯內容時修改或新增視覺化片段，請按一下&#x200B;**重新整理**&#x200B;圖示，以最新變更更新清單。

1. 從清單拖放任何視覺化片段到您要插入它的區域。 如同任何其他元件，您可以在內容中移動片段。

1. 選取片段以在右窗格中顯示其選項。

   ![在右窗格中顯示片段選項的熒幕擷圖](assets/fragment-right-pane.png)

   從&#x200B;**[!UICONTROL 設定]**&#x200B;索引標籤，您可以：

   * 選擇您要顯示片段的裝置。
   * 按一下&#x200B;**編輯內容**&#x200B;按鈕，開啟此片段的內容。 [了解更多](../content/fragments.md#edit-fragments)

     您可以使用&#x200B;**[!UICONTROL 樣式]**&#x200B;索引標籤進一步自訂您的片段。

1. 如有需要，請中斷具有原始視覺化片段的繼承。 [了解更多](#break-inheritance)

   您也可以從內容中刪除片段或加以複製。 直接從顯示於片段頂端的內容功能表執行這些動作。

1. 視需要新增儘可能多的視覺化片段，並&#x200B;**[!UICONTROL 儲存]**&#x200B;您的變更。

### 唯讀模式下的視覺化片段 {#fragment-readonly}

存取權可套用至視覺片段。

如果未授予特定視覺化片段的許可權版本，內容範本會以&#x200B;**唯讀模式**&#x200B;顯示。 在此情況下，**[!UICONTROL 編輯內容]**&#x200B;按鈕會取代為&#x200B;**[!UICONTROL 檢視內容]**&#x200B;按鈕，可讓您檢視片段而不做變更。

![以唯讀模式顯示視覺化片段的熒幕擷圖](assets/fragment-readonly.png){zoomable="yes"}

如下所示，所有功能圖示都會停用，限制僅供檢視互動。

![以唯讀模式顯示已停用功能圖示的熒幕擷圖](assets/fragment-readonly-view.png){zoomable="yes"}

## 中斷繼承 {#break-inheritance}

當您編輯視覺片段時，變更會同步化並自動傳播至包含該片段的所有電子郵件傳遞和內容範本。

依預設，片段在新增至電子郵件或內容範本時會進行同步。

不過，您可以中斷原始片段的繼承。 在這種情況下，片段的內容會複製到目前的設計中，且變更不再同步。

若要中斷繼承，請遵循下列步驟：

1. 選取視覺片段。

1. 按一下內容工具列中的解鎖圖示。

   ![顯示解除鎖定圖示以中斷繼承的熒幕擷圖](assets/fragment-break-inheritance.png)

1. 片段會成為不再連結至原始片段的獨立元素。 編輯它，就像內容中的任何其他內容元件一樣。 [了解更多](../email/content-components.md)