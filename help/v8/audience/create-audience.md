---
audience: end-user
title: 建立和管理對象
description: 瞭解如何在Adobe Campaign Web中建立和管理對象
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 1%

---


# 建立對象 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="對象"
>abstract="您可以從此畫面存取傳遞中可鎖定目標的所有對象清單。 按一下 **建立** 使用各種工作流程活動(例如 **Split** 或 **排除**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="對象設定"
>abstract="輸入對象名稱和其他選項，然後按一下 **建立對象** 按鈕。"

Campaign Web可讓您在視覺工作流程畫布中建立新對象。 除了從頭開始建立簡單的對象外，您也可以運用工作流程活動來調整對象。 例如，您可以將多個受眾合併為單一受眾、使用外部屬性豐富受眾，或根據您選擇的規則將受眾分割為多個受眾。

當您完成工作流程後，產生的對象會自動與您現有的對象一起儲存在Campaign資料庫中。 然後便可在行銷活動或獨立傳送中鎖定這些對象。

## 建立您的第一個對象 {#create}

若要建立對象，請遵循下列步驟：

1. 導覽至 **[!UICONTROL 受眾]** 功能表，然後按一下 **[!UICONTROL 建立對象]** 按鈕的位置。
1. 為對象提供標籤。
1. 展開 **[!UICONTROL 其他選項]** 區段來設定進階對象引數。

   依預設，對象會建立到 **[!UICONTROL 設定檔和目標]** / **[!UICONTROL 清單]** explorer功能表。 您可以使用變更預設儲存位置 **[!UICONTROL 資料夾]** 欄位。

   ![](assets/audiences-settings.png)

1. 設定對象設定後，請按一下 **[!UICONTROL 建立對象]** 按鈕。 工作流程畫布隨即顯示，其中包含兩個預設活動：

   * **[!UICONTROL 建立對象]**：這是工作流程的起點，可讓您建立受眾，並將其用作工作流程的基礎。

   * **[!UICONTROL 儲存對象]**：這代表工作流程的最後一步，可讓您將工作流程結果儲存為新對象。

1. 開啟 **[!UICONTROL 建立對象]** 活動，並使用規則產生器，透過篩選資料庫中所包含的資料，定義要包含在對象中的母體。 [瞭解如何設定建置對象活動](../workflows/activities/build-audience.md)

1. 如果您想要對目標母體執行其他作業至工作流程，請視需要新增許多活動，並將它們連線在一起。 有關如何設定工作流程活動的詳細資訊，請參閱 [工作流程檔案](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >管道活動不適用於對象工作流程。

   ![](assets/audience-creation-canvas.png)

1. 設定 **[!UICONTROL 儲存對象]** 活動，指定您想要如何儲存工作流程中上游運算的母體。 [瞭解如何設定「儲存對象」活動](../workflows/activities/save-audience.md)

1. 當工作流程準備就緒時，按一下 **[!UICONTROL 開始]** 以執行。

工作流程會儲存在 **[!UICONTROL 工作流程]** 清單，而可在中存取產生的對象 **[!UICONTROL 受眾]** 清單。

## 對象工作流程範例 {#example}

以下範例顯示一個受眾工作流程，其設定是針對住在紐約的女客戶，並根據她們的最新購買專案（瑜伽或奔跑裝備）建立兩個新受眾。

![](assets/audiences-example.png)

1. 此 **[!UICONTROL 建立對象]** 活動目標是住在紐約的所有女性設定檔。
1. 此 **[!UICONTROL 擴充]** 活動可透過「購買」表格中的資訊來識別客戶購買的產品型別，藉此豐富受眾。
1. 此 **[!UICONTROL Split]** 活動會根據客戶的最新購買情況，將工作流程分為兩個路徑。
1. 此 **[!UICONTROL 儲存對象]** 每個路徑結尾的活動會在資料庫中建立兩個新對象，包括每個路徑中計算的母體。

## 監視和管理對象 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="對象錯誤"
>abstract="對象資料無法使用。 請等候工作流程執行結束。"

Campaign網頁適用的對象清單可從 **[!UICONTROL 受眾]** 功能表。

![](assets/audiences-list.png)

對象可以源自多個來源。 此 **[!UICONTROL 來源]** 欄表示建立特定對象的位置：

* **[!UICONTROL Adobe Campaign]**：這些對象是在Adobe Campaign V8主控台中建立。 進一步瞭解 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform：]** 這些對象是在Adobe Experience Platform中建立，並使用Adobe來源和目的地整合整合來整合至Campaign網頁。 瞭解如何在中設定這項整合 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**：這些對象是使用Campaign Web對象工作流程建立的。 [瞭解如何建立對象](create-audience.md)

若要取得對象的詳細資訊，請從清單中將其開啟。 對象屬性會連同對象中包含的設定檔數量一起顯示。 您可以隨時使用 **[!UICONTROL 計算]** 按鈕。

此 **[!UICONTROL 資料]** 索引標籤可讓您檢視屬於受眾的設定檔。 您可以新增更多欄或運用進階篩選器來調整顯示的資料，以自訂此檢視。

![](assets/audiences-details.png)

若要複製或刪除對象，請按一下 **[!UICONTROL 更多動作]** 「對象」清單中「對象名稱」旁或「對象詳細資料」畫面內的可用按鈕。
