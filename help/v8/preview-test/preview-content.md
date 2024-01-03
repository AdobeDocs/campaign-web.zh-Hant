---
audience: end-user
title: 預覽傳遞內容
description: 瞭解如何使用Campaign Web UI預覽您的傳遞內容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="有限可用性"
source-git-commit: 6dcdfae8aa6d6346fc02217db77a96cf6d219fdc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 1%

---


# 預覽傳遞內容 {#preview-content}

使用 [!DNL Campaign] 內容模擬功能，可在傳送訊息前預覽訊息內容。 這可讓您控制個人化，並檢查其向收件者顯示的方式。

若要預覽傳送的內容，請遵循下列步驟。

1. 瀏覽至傳送的編輯內容畫面或 [電子郵件設計工具](../content/get-started-email-designer.md).

1. 按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/simulate-button.png)

1. 若要選取將用來預覽個人化內容的設定檔，請使用：

   * **[!UICONTROL 新增測試設定檔]** 用於預覽電子郵件和簡訊傳遞

   * **[!UICONTROL 新增訂閱者]** 預覽推播通知

1. 您可以合併測試設定檔和設定檔，以預覽您的電子郵件或簡訊訊息。

   * 此 **[!UICONTROL 測試設定檔]** tab會列出所有種子地址，這些地址是資料庫中的其他虛構收件者。

     ![](assets/simulate-select-profiles.png)

     >[!NOTE]
     >
     >測試設定檔可從以下網址建立： **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 功能表。 [了解更多](../audience/test-profiles.md#create-test-profiles)

   * 此 **[!UICONTROL 設定檔]** 索引標籤會列出所有儲存在 **[!UICONTROL 設定檔和目標]** 資料夾來自 [!DNL Campaign] 主控台。 進一步瞭解 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}.

     >[!NOTE]
     >
     >您也可以從Campaign網頁UI中的對應索引標籤，檢視及管理設定檔。 [了解更多](../audience/about-recipients.md)

1. 按一下 **[!UICONTROL 選取]** 以確認您的選取。

   傳遞內容的預覽會顯示在 **[!UICONTROL 模擬]** 畫面。 個人化元素會取代為左側窗格中選取之設定檔的資料。

   ![](assets/simulate-preview.png)

1. 如果您已新增多個設定檔，您可以在清單中的設定檔之間切換，以預覽對應的傳送內容。 您也可以使用左窗格中的對應按鈕，新增更多測試設定檔並清除選取專案。

1. 對於電子郵件傳遞，您可以調整 **[!UICONTROL 縮放等級]** 並使用右上角的專用圖示在案頭或行動裝置上預覽您的內容。

1. 從 **[!UICONTROL 模擬]** 熒幕您也可以：
   * 傳送測試傳遞至特定收件者進行驗證 —  [瞭解更多](test-deliveries.md)
   * 存取已傳送測試傳送的記錄 —  [瞭解更多](test-deliveries.md#access-test-deliveries)
   * 僅針對電子郵件，請檢查常見電子郵件使用者端中的訊息內容呈現 —  [瞭解更多](email-rendering.md)



