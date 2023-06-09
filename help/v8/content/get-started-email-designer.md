---
audience: end-user
title: 編輯電子郵件內容
description: 瞭解如何在Campaign Web UI中使用電子郵件設計工具開始建立內容
badge: label="Alpha" type="Positive"
source-git-commit: 97c65771f9302bb188de0a8dae05f0d607519d4a
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 9%

---

# 開始使用電子郵件設計工具 {#get-started-email-designer}

在 Adobe Campaign 中建立電子郵件後，您必須定義其內容。

電子郵件設計工具可讓您透過直覺式的拖放介面，建立吸引人、個人訂做的電子郵件。 無論您是從空白顯示窗開始、匯入現有內容或運用現有範本，針對每封電子郵件（無論是促銷或異動）設計和調整所有內容。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* 使用 [!DNL Campaign] 電子郵件設計功能，可輕鬆建立回應式電子郵件。 [了解更多](create-email-content.md)

* 根據客戶的設定檔屬性建立個人化，以增強客戶體驗。 [了解更多](../personalization/personalize.md)

* 設定條件式內容欄位，以根據收件者的設定檔建立動態個人化。 [了解更多](../personalization/conditions.md)

## 電子郵件設計最佳實務 {#best-practices}

傳送電子郵件時，請務必考慮收件者可能會轉寄電子郵件，這有時會導致電子郵件的轉譯發生問題。 使用電子郵件提供者不支援轉送的CSS類別時，尤其如此，例如，如果您使用「is-desktop-hidden」CSS類別來隱藏行動裝置上的影像。

若要將這些轉譯問題降至最低，建議您儘可能簡化電子郵件設計結構。 請嘗試使用適用於案頭和行動裝置的單一設計，並避免使用複雜的CSS類別或其他設計元素，因為並非所有電子郵件使用者端都完全支援這些元素。 透過遵循這些最佳實務，您可以協助確保您的電子郵件可一致地正確呈現，無論收件者如何檢視或轉寄電子郵件。

## 開始編寫您的內容 {#start-authoring}

從電子郵件傳遞控制面板，前往 [編輯內容](edit-content.md) 畫面以開啟「電子郵件設計工具」首頁。 從那裡，從下列選項中選擇您要如何設計電子郵件：

* **從頭開始設計您的電子郵件** 透過電子郵件設計工具的介面。 瞭解如何在中設計您的電子郵件內容 [本節](create-email-content.md).

* **程式碼或貼上原始HTML** 直接在電子郵件設計工具中建立。 瞭解如何在中編寫您自己的內容 [本節](code-content.md).

* **匯入現有HTML內容** 從檔案或.zip資料夾。 瞭解如何在中匯入電子郵件內容 [本節](existing-content.md).

* **選取現有內容** 內建或自訂範本清單中的。 瞭解如何使用電子郵件範本 [本節](email-templates.md).

  ![](assets/email_designer_create_options.png)

