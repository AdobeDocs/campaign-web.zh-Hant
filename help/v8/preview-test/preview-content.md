---
audience: end-user
title: 預覽傳遞內容
description: 瞭解如何使用Campaign Web UI預覽您的傳遞內容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha"
source-git-commit: 861a16500b5faf947dd1545976f3c4bbe6548467
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 10%

---


# 預覽傳遞內容 {#preview-content}

使用 [!DNL Campaign] 內容模擬功能，可在傳送訊息前預覽訊息內容。 這可讓您控制個人化，並檢查其向收件者顯示的方式。

若要預覽傳送內容，請遵循下列步驟。

1. 瀏覽至傳送的編輯內容畫面。

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. 按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/simulate-button.png)

1. 若要選取將用來預覽個人化內容的設定檔，請使用：

   * **[!UICONTROL 新增測試設定檔]** 預覽電子郵件和簡訊訊息

   * **[!UICONTROL 新增訂閱者]** 用於預覽推播傳遞

1. 您可以合併測試設定檔和設定檔，以預覽您的電子郵件或簡訊訊息。

   * 「**[!UICONTROL 測試設定檔]**」索引標籤會列出所有種子地址，這些地址是資料庫中額外和虛構的收件者。

     >[!NOTE]
     >
     >測試設定檔可在 [!DNL Campaign] 主控台進入 **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子地址]** 資料夾。 進一步瞭解 [Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * 「**[!UICONTROL 設定檔]**」索引標籤會列出儲存在 主控台「**[!UICONTROL 設定檔和目標]**」資料夾中的所有收件者。[!DNL Campaign][了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. 按一下 **[!UICONTROL 選取]** 以確認您的選取。

   傳遞內容的預覽會顯示在 **[!UICONTROL 模擬]** 畫面。 個人化元素會以來自在左窗格中選取之設定檔的資料取代。

   ![](assets/simulate-preview.png)

1. 如果您已新增多個設定檔，您可以在清單中的多個設定檔之間切換，以預覽對應的傳送內容。 您也可以使用左窗格中的對應按鈕，新增更多測試設定檔並清除選取專案。

1. 對於電子郵件傳送，您可以調整 **[!UICONTROL 縮放等級]** 並使用右上角的專用圖示在案頭或行動裝置上預覽您的內容。

1. 從 **[!UICONTROL 模擬]** 熒幕您也可以：
   * 傳送測試傳遞至特定收件者進行驗證 —  [瞭解更多](proofs.md)
   * 存取已傳送測試傳送的記錄 —  [瞭解更多](proofs.md#access-proofs)
   * 僅針對電子郵件，請檢查常見電子郵件使用者端中的訊息內容呈現 —  [瞭解更多](email-rendering.md)



