---
audience: end-user
title: 預覽傳遞內容
description: 瞭解如何使用Campaign網頁使用者介面預覽您的傳遞內容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---

# 預覽訊息內容。 {#preview-content}

使用[!DNL Campaign]內容模擬功能，在傳送訊息之前預覽訊息內容。 此功能可讓您控制個人化，並檢查向收件者顯示訊息的方式。

若要預覽傳送的內容，請執行下列步驟：

1. 瀏覽至您傳送的編輯內容畫面或[電子郵件Designer](../email/get-started-email-designer.md)。

1. 按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕。

   ![顯示模擬內容按鈕的影像](assets/simulate-button.png){zoomable="yes"}

1. 選取要用於預覽內容的設定檔。 若要執行此動作，請按一下&#x200B;**[!UICONTROL 新增測試設定檔]**&#x200B;按鈕（適用於電子郵件和簡訊）或&#x200B;**[!UICONTROL 新增訂閱者]**&#x200B;按鈕（適用於推播通知）。

1. 結合設定檔和測試設定檔，以預覽您的電子郵件或簡訊訊息。

   * **[!UICONTROL 測試設定檔]**&#x200B;索引標籤會列出所有測試設定檔，這些設定檔是資料庫中的其他虛構收件者。 [瞭解如何使用測試設定檔](../audience/test-profiles.md)。

   * **[!UICONTROL 設定檔]**&#x200B;索引標籤會列出儲存在資料庫中的所有設定檔。 [瞭解如何使用設定檔](../audience/about-recipients.md)。

   ![影像顯示選取的設定檔](assets/simulate-select-profiles.png){zoomable="yes"}

1. 瀏覽測試設定檔或設定檔清單時，請使用篩選器來縮小您的搜尋範圍。 例如，定義規則以尋找所有狀態為&#x200B;**[!UICONTROL 潛在客戶]**&#x200B;的測試設定檔。 [瞭解如何使用查詢模型工具](../query/query-modeler-overview.md)來新增規則。

   ![顯示套用至測試設定檔之篩選器的影像](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 選取]**&#x200B;以確認您的選取。

   傳遞內容的預覽會顯示在&#x200B;**[!UICONTROL 模擬]**&#x200B;畫面的右窗格中。 個人化元素會取代為左側窗格中選取之設定檔的資料。

   ![顯示傳遞內容預覽的影像](assets/simulate-preview.png){zoomable="yes"}

1. 如果新增多個設定檔，請在清單中的設定檔之間切換，以預覽對應的傳送內容。 使用左窗格中的對應按鈕，新增更多測試設定檔或清除您的選取專案。

1. 對於電子郵件傳遞，請調整&#x200B;**[!UICONTROL 縮放等級]**，並使用右上角的專用圖示在桌上型電腦或行動裝置上預覽您的內容。

1. 從&#x200B;**[!UICONTROL Simulate]**&#x200B;畫面，您也可以：
   * 傳送校樣給特定收件者進行驗證 — [瞭解更多](test-deliveries.md)。
   * 存取已傳送校樣的記錄檔 — [深入瞭解](test-deliveries.md#access-test-deliveries)。
   * 僅針對電子郵件，請檢查常見電子郵件使用者端中的郵件內容呈現 — [深入瞭解](email-rendering.md)。