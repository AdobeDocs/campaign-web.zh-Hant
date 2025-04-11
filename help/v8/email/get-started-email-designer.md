---
audience: end-user
title: 編輯電子郵件內容
description: 了解如何使用 Campaign Web 使用者介面中的電子郵件設計工具開始建置您的內容
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 45%

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

若要將這些轉譯問題降至最低，請儘可能簡化您的電子郵件設計結構。 請使用適用於案頭和行動裝置的單一設計，並避免使用複雜的CSS類別或其他設計元素，因為並非所有電子郵件使用者端都完全支援這些元素。 透過遵循這些最佳實務，有助於確保您的電子郵件可一致地呈現，無論收件者如何檢視或轉寄電子郵件。

## 開始編寫您的內容  {#start-authoring}

從電子郵件傳遞儀表板，經過[編輯內容](edit-content.md)畫面，以開啟電子郵件設計工具首頁。從那裡，可由下列選項中選擇您要如何設計您的電子郵件：

* 透過電子郵件設計工具的介面&#x200B;**從頭開始設計您的電子郵件**。若要了解如何設計您的電子郵件內容，請參閱[本章節](create-email-content.md)。

* 直接在電子郵件設計工具中&#x200B;**編寫程式碼或貼上原始 HTML**。若要了解如何將您自己的內容編寫程式碼，請參閱[本章節](code-content.md)。

* 從檔案或 .zip 資料夾&#x200B;**匯入現有的 HTML 內容**。瞭解如何在[本節](existing-content.md)中匯入電子郵件內容。

* 從內建或自訂範本清單中&#x200B;**選取現有內容**。在[本節](create-email-templates.md)中瞭解如何使用電子郵件範本。

  ![電子郵件Designer介面中可用於建立電子郵件內容的選項](assets/email_designer_create_options.png){zoomable="yes"}
