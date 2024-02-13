---
audience: end-user
title: 預覽傳遞內容
description: 瞭解如何使用Campaign網頁使用者介面預覽您的傳遞內容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 8667de1d86428427edd9a2718218de9801b0922d
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---


# 預覽訊息內容。 {#preview-content}

使用 [!DNL Campaign] 內容模擬功能，可在傳送訊息前預覽訊息內容。 這可讓您控制個人化，並檢查其向收件者顯示的方式。

若要預覽傳送的內容，請遵循下列步驟。

1. 瀏覽至傳送的編輯內容畫面或 [電子郵件設計工具](../email/get-started-email-designer.md).

1. 按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/simulate-button.png){zoomable=&quot;yes&quot;}

1. 選取要用來預覽內容的設定檔。 若要這麼做，請按一下 **[!UICONTROL 新增測試設定檔]** 按鈕（適用於電子郵件和簡訊）或 **[!UICONTROL 新增訂閱者]** 按鈕（用於推播通知）。

1. 您可以合併設定檔和測試設定檔，以預覽您的電子郵件或簡訊訊息。

   * 此 **[!UICONTROL 測試設定檔]** 索引標籤會列出所有測試設定檔，這些是資料庫中的其他虛構收件者。 [瞭解如何使用測試設定檔](../audience/test-profiles.md)

   * 此 **[!UICONTROL 設定檔]** 索引標籤會列出儲存在資料庫中的所有設定檔。 [瞭解如何使用設定檔](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable=&quot;yes&quot;}

1. 瀏覽測試設定檔或設定檔清單時，您可以使用篩選器來縮小搜尋範圍。 例如，您可以定義規則以尋找所有具有 **[!UICONTROL 潛在客戶]** 狀態。 [瞭解如何使用查詢建模器新增規則](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. 按一下 **[!UICONTROL 選取]** 以確認您的選取。

   傳遞內容的預覽會顯示在 **[!UICONTROL 模擬]** 畫面。 個人化元素會取代為左側窗格中選取之設定檔的資料。

   ![](assets/simulate-preview.png){zoomable=&quot;yes&quot;}

1. 如果您已新增多個設定檔，您可以在清單中的設定檔之間切換，以預覽對應的傳送內容。 您也可以使用左窗格中的對應按鈕，新增更多測試設定檔並清除選取專案。

1. 對於電子郵件傳遞，您可以調整 **[!UICONTROL 縮放等級]** 並使用右上角的專用圖示在案頭或行動裝置上預覽您的內容。

1. 從 **[!UICONTROL 模擬]** 熒幕您也可以：
   * 傳送測試傳遞至特定收件者進行驗證 —  [瞭解更多](test-deliveries.md)
   * 存取已傳送測試傳送的記錄 —  [瞭解更多](test-deliveries.md#access-test-deliveries)
   * 僅針對電子郵件，請檢查常見電子郵件使用者端中的訊息內容呈現 —  [瞭解更多](email-rendering.md)



