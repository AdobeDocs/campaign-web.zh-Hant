---
audience: end-user
title: 編輯電子郵件內容
description: 了解如何使用 Campaign Web 使用者介面中的電子郵件設計工具開始建置您的內容
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: d7fc756b2e1d94b43c76ced748e1bf7c7ae5da0d
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 61%

---


# 開始使用電子郵件設計工具 {#get-started-email-designer}

在Adobe Campaign中建立電子郵件後，您需要定義其內容。

電子郵件設計工具讓您能夠透過直覺式的拖放介面建立引人入勝、量身打造的客製化電子郵件。無論您是從空白顯示窗開始、匯入現有內容或運用現有範本，針對每封電子郵件（不論是促銷或異動）設計和調整所有內容。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* 使用[!DNL Campaign]電子郵件設計功能，可輕鬆建置回應式電子郵件。[了解更多](create-email-content.md)

* 根據客戶設定檔屬性建立個人化電子郵件，以增強客戶體驗。 [了解更多](../personalization/personalize.md)

* 設定條件式內容欄位以根據收件者的輪廓建立動態個人化。[了解更多](../personalization/conditions.md)

## 電子郵件設計最佳做法 {#best-practices}

傳送電子郵件時，請考量收件者可能會轉寄電子郵件，這有時會導致電子郵件轉譯發生問題。 使用用於轉送的電子郵件提供者可能不支援的CSS類別時，尤其如此。 例如，如果您使用「is-desktop-hidden」CSS類別來隱藏行動裝置上的影像，該類別可能無法正確呈現。

為了盡量減少這些呈現問題，我們建議保持您的電子郵件設計結構盡可能簡單。可嘗試使用同時適用於桌上型電腦和行動裝置的單一設計，並且避免使用複雜的 CSS 類別或其他並非所有電子郵件用戶端都可完全支援的設計元素。在電子郵件中使用影像時，請避免使用大於2 MB的影像或使用編碼的影像連結。

若能按照這些最佳做法進行，即有助於確保電子郵件會始終如一地正確呈現，無論收件者以什麼方式檢視或轉寄。

## 開始編寫您的內容  {#start-authoring}

從電子郵件傳遞儀表板，經過[編輯內容](edit-content.md)畫面，以開啟電子郵件設計工具首頁。從那裡，可由下列選項中選擇您要如何設計您的電子郵件：

* 透過電子郵件設計工具的介面&#x200B;**從頭開始設計您的電子郵件**。若要了解如何設計您的電子郵件內容，請參閱[本章節](create-email-content.md)。

* 直接在電子郵件設計工具中&#x200B;**編寫程式碼或貼上原始 HTML**。若要了解如何將您自己的內容編寫程式碼，請參閱[本章節](code-content.md)。

* 從檔案或 .zip 資料夾&#x200B;**匯入現有的 HTML 內容**。瞭解如何在[本節](existing-content.md)中匯入電子郵件內容。

* 從內建或自訂範本清單中&#x200B;**選取現有內容**。在[本節](create-email-templates.md)中瞭解如何使用電子郵件範本。

  ![電子郵件Designer介面中可用於建立電子郵件內容的選項](assets/email_designer_create_options.png){zoomable="yes"}
