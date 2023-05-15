---
title: 在 Campaign 中個人化您的內容
description: 了解如何在 Adobe Campaign Web UI 中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 05d87fc9ff8f5e2038eba4cc9438e058566e04c8
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 95%

---


# 個人化您的內容{#add-personalization}

您可以透過以下方式個人化訊息內容：

* 插入動態&#x200B;**個人化欄位**

   個人化欄位用於訊息的第一層個人化。您可以從個人化編輯器選取資料庫中的任何欄位。對於傳遞，您可以選取與收件者、訊息或傳遞相關的任何欄位。這些個人化屬性可以插入訊息的主旨行或內文中。

   ![](assets/perso-subject-line.png)

   以下語法將收件者城市插入您的內容：&lt;%= recipient.location.city %>。

* 插入預先定義的&#x200B;**內容區塊**

   Campaign 隨附一組個人化區塊，其中包含您可以插入到傳遞中的特定轉譯。例如，您可以新增標誌、問候訊息或訊息鏡像頁面的連結。內容區塊可從個人化編輯器的專屬項目取得。

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->


內建的內容區塊包括：

* **[!UICONTROL 由 Adobe Campaign 啟用]**：插入「由 Adobe Campaign 啟用」標誌。
* **[!UICONTROL 專有名詞的格式化函數]**：產生 **[!UICONTROL toSmartCase]** Javascript 函數，它將每個單詞的第一個字母變更為大寫。
* **[!UICONTROL 問候語]**：插入帶有收件人全名的問候語，後面跟著一個逗號。範例：「你好 John Doe，」。
* **[!UICONTROL 插入標誌]**：插入在執行個體中定義的標誌。
* **[!UICONTROL 鏡像頁面連結]**：插入[鏡像頁面](../content/mirror-page.md)的連結。預設格式：「如果您無法正確檢視此訊息，請按一下此處」。
* **[!UICONTROL 鏡像頁面 URL]**：插入鏡像頁面 URL，使傳遞設計工具檢查連結。
* **[!UICONTROL 單一模式的優惠接受 URL]**：插入可以將優惠設定為&#x200B;**[!UICONTROL 接受]** 的 URL。(如果啟用互動模組，則此區塊可用)
* **[!UICONTROL 註冊確認]**：插入可以確認訂閱的連結。
* **[!UICONTROL 註冊連結]**：插入訂閱連結。此連結在執行個體設定中定義。預設內容：「若要註冊，請按一下這裡。」
* **[!UICONTROL 註冊連結 (含推薦者)]**：插入可以識別訪客和傳遞的訂閱連結。此連結在執行個體設定中定義。
* **[!UICONTROL 註冊頁面 URL]**：插入訂閱 URL
* **[!UICONTROL 內容電子郵件的樣式]**&#x200B;和&#x200B;**[!UICONTROL 通知樣式]**：產生使用預先定義的 HTML 樣式格式化電子郵件的程式碼。
* **[!UICONTROL 取消訂閱連結]**：插入可以取消訂閱所有傳遞 (封鎖清單) 的連結。預設關聯內容：「您收到此訊息因為您曾聯絡&#x200B;***您的組織名稱***&#x200B;或附屬機構。若不要再收到來自&#x200B;***您的組織名稱***&#x200B;的訊息，請按一下這裡。」

## 個人化電子郵件主旨行 {#personalize-subject-line}

若要在訊息的&#x200B;**[!UICONTROL 主旨行]**&#x200B;欄位新增個人化，請依照以下步驟操作：

1. 按一下「**[!UICONTROL 主旨行]**」欄位右側的「**[!UICONTROL 開啟個人化對話框]**」圖示。

   ![](assets/perso-subject.png){width="600"}

1. 輸入主旨行內容，然後選取要新增的個人化屬性。

1. 按一下 **[!UICONTROL 確認]****驗證。 個人化屬性已新增到主旨行。

## 個人化您的電子郵件內容 {#personalize-emails}

若要個人化電子郵件內容，請在電子郵件設計工具中開啟訊息，然後：

1. 在文字區塊內按一下。
1. 在內容關聯式工具列中，選取「**[!UICONTROL 新增個人化]**」。

   ![](assets/perso-add-to-content.png)

1. 在個人化編輯器中插入收件者名稱並確認。

   ![](assets/perso-add-name.png)

   個人化屬性已新增到電子郵件內容。

   您可以模擬內容以檢查轉譯。[了解更多](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. 若要在電子郵件中新增內容區塊，請執行相同的步驟，然後從最後一個圖示選取內容區塊：

   ![](assets/perso-insert-block.png)

1. 插入後，內容區塊會新增至電子郵件內容。在傳送準備步驟中，當產生個人化時，內容區塊會自動適應收件者設定檔。

   ![](assets/perso-content-block-in-email.png)

## 個人化電子郵件中的連結 {#personalize-links}

若要個人化&#x200B;**連結**：

1. 選取文字區塊或影像。
1. 在內容關聯式工具列中，選取「**插入連結**」。

   ![](assets/perso-link.png)

1. 輸入連結標籤並使用「**插入連結**」按鈕來個人化連結。

   ![](assets/perso-link-insert-icon.png)

1. 使用個人化編輯器來定義和個人化連結，並確認。

   ![](assets/perso-link-edit.png)


## 個人化您的優惠 {#personalize-offers}

您也可以在將文字類型的內容新增到優惠的表示時存取個人化編輯器。在[本章節](../content/offers.md)了解更多資訊。
