---
audience: end-user
title: 測試電子郵件轉譯
description: 瞭解如何在Campaign網頁使用者介面中測試電子郵件呈現
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 2%

---

# 測試電子郵件轉譯 {#email-rendering}

在傳送電子郵件之前，請確定您的訊息在各種Web使用者端與裝置間以最佳方式向收件者顯示。

若要達成此目的，請使用[!DNL Adobe Campaign]中您的&#x200B;**Litmus**&#x200B;帳戶，在不同的內容中立即預覽電子郵件呈現。 這可讓您檢查與主要案頭應用程式、網頁郵件服務、行動裝置等的相容性。

>[!CAUTION]
>
>在Campaign中使用電子郵件呈現會將校樣傳送至協力廠商系統。 將您的Litmus帳戶與[!DNL Campaign]連線即表示您確認Adobe對您可能傳送給該協力廠商的任何資料概不負責。 Litmus的電子郵件資料保留原則適用於這些電子郵件，包括可能包含在這些校樣中的個人化資料。 若要存取或刪除這類資料，請直接聯絡Litmus。

若要存取電子郵件呈現功能，請完成下列必要條件：

* 擁有Litmus帳戶。
* 選取設定檔及/或測試設定檔。 在[本節](preview-content.md)中瞭解如何操作。

然後，請遵循以下步驟。

1. 在[編輯內容](../email/edit-content.md)畫面或[電子郵件Designer](../email/get-started-email-designer.md)中，按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕。

1. 選取&#x200B;**[!UICONTROL 轉譯電子郵件]**&#x200B;按鈕。

   在電子郵件編輯器中![模擬內容按鈕](assets/simulate-rendering-button.png){zoomable="yes"}

1. 按一下右上角的&#x200B;**連線您的Litmus帳戶**。

   電子郵件轉譯介面中的![Litmus帳戶連線選項](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. 輸入您的認證並登入。

   ![Litmus帳戶登入畫面](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. 按一下&#x200B;**執行測試**&#x200B;按鈕以產生電子郵件預覽。

1. 在熱門的桌上型電腦、行動裝置和網頁型使用者端中檢閱您的電子郵件內容。

   ![跨不同使用者端以電子郵件呈現預覽](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile, and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![Preview pane showing email rendering across selected clients](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->