---
audience: end-user
title: 建立對象
description: 瞭解如何在Adobe Campaign Web中建立對象
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# 建立對象 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="對象"
>abstract="您可以從此畫面建立受眾，並將受眾合併至視覺畫布中。 新增各種工作流程活動，例如 **Split** 或 **排除** 以產生新的和完善的對象。"

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="對象設定"
>abstract="輸入對象名稱和其他選項，然後按一下 **建立對象** 按鈕。"

Campaign Web可讓您在視覺工作流程畫布中建立新對象。 除了從頭開始建立簡單的對象之外，您還可以運用工作流程活動來調整對象。 例如，您可以將多個受眾分成單一受眾、使用外部屬性豐富受眾，或將特定受眾分成多個受眾。

當您完成工作流程後，產生的對象會自動與您現有的對象一起儲存在Campaign資料庫中。 然後便可在行銷活動或獨立傳送中鎖定這些對象。

建立對象的主要步驟如下：

1. 建立對象工作流程。
1. 設定「建立對象」活動，以根據您的需求查詢資料庫。
1. 新增工作流程活動以精簡您的對象（選用）。
1. 設定「儲存對象」活動。
1. 執行工作流程，將產生的對象儲存至資料庫。


## 建立您的第一個對象 {#create}

若要建立對象，請遵循下列步驟：

1. 導覽至 **[!UICONTROL 受眾]** 功能表，然後按一下 **[!UICONTROL 建立對象]** 按鈕的位置。
1. 為對象提供標籤。
1. 展開 **[!UICONTROL 其他選項]** 區段來設定進階對象引數。

   依預設，對象會建立到 **[!UICONTROL 設定檔和目標]** / **[!UICONTROL 清單]** explorer功能表。 您可以使用變更預設儲存位置 **[!UICONTROL 資料夾]** 欄位。

   ![](assets/audiences-settings.png)

1. 設定對象設定後，請按一下 **[!UICONTROL 建立對象]** 按鈕。

1. 工作流程畫布隨即顯示，其中包含兩個預設活動：

   * **[!UICONTROL 建立對象]**：這是工作流程的起點，可讓您建立受眾，並將其用作工作流程的基礎。 [瞭解如何設定建置對象活動](../workflows/activities/build-audience.md)

   * **[!UICONTROL 儲存對象]**：這代表工作流程的最後一步，可讓您將結果儲存為新對象。 [瞭解如何設定「儲存對象」活動](../workflows/activities/save-audience.md)

1. 如果您想在 **[!UICONTROL 建立對象]** 活動，視需要在工作流程中新增儘可能多的活動。 有關如何設定工作流程活動的詳細資訊，請參閱 [工作流程檔案](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >管道活動不適用於對象工作流程。

   ![](assets/audience-creation-canvas.png)

1. 當工作流程準備就緒時，按一下 **[!UICONTROL 開始]** 以執行。

1. 工作流程會儲存在 **[!UICONTROL 工作流程]** 清單，而可在中存取產生的對象 **[!UICONTROL 受眾]** 清單。 [瞭解如何監視和管理對象](access-audiences.md)

## 對象工作流程範例 {#example}

以下範例顯示一個受眾工作流程，其設定是針對住在紐約的女客戶，並根據她們在「瑜伽」或「奔跑」用具中的興趣中心來建立兩個新受眾。 這兩個受眾已新增有關客戶購買的其他資訊而更加豐富。

新增熒幕擷圖

1. 「建立對象」活動會鎖定住在紐約的所有女性設定檔。
1. 「擴充」活動使用「購買」表格中的屬性來豐富對象。
1. 「分割」活動會根據客戶的興趣中心將工作流程劃分為兩個路徑。
1. 在每個路徑結尾的「儲存對象」活動，將每個對象儲存至資料庫。
