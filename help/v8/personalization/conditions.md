---
title: 建立條件式內容
description: 瞭解如何定義條件以在Adobe Campaign網頁中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f6e3fc0da05ecc2fda158c970458cc702b27079c
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 6%

---

# 建立條件內容{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="新增條件內容"
>abstract="設定條件內容欄位，以根據收件者的設定檔資料建立進階的動態個人化。在滿足特定條件時，會更換訊息內容中的文字區塊、連結、主題行和/或影像。"

## 開始使用條件式內容 {#gs}

條件式內容是一項強大的功能，可讓您根據收件者的設定檔資料建立動態個人化，在滿足某些條件時自動取代文字區塊和影像。 此功能可以將您的行銷活動提升到新的高度，並為您的客群提供目標明確的個人化體驗。

例如，透過設定條件式內容欄位，您可以根據收件者的設定檔建立進階動態個人化。 當滿足特定條件時，會在訊息內容中取代文字區塊、連結、主旨行和/或影像。 例如，您可以根據Adobe Campaign資料庫中性別欄位的值顯示「先生」或「夫人」，或根據收件者偏好的語言包含其他連結。

若要建立條件式內容，您必須使用特定協助程式函式，在&#x200B;**運算式編輯器**&#x200B;中建立條件。 此方法適用於所有傳遞管道，以及任何可存取運算式編輯器的欄位，例如主旨行或電子郵件連結及文字/按鈕內容元件。 [瞭解如何存取運算式編輯器](gs-personalization.md#access)

除了運算式編輯器之外，在設計可讓您為電子郵件內文的元素建立多個變體的電子郵件時，還可以利用專用的&#x200B;**條件式內容產生器**。 [瞭解如何在電子郵件中建立條件式內容](#condition-condition-builder)

## 在運算式編輯器中建立條件 {#condition-perso-editor}

若要使用運算式編輯器定義傳遞的條件式內容，請遵循下列步驟。 在此範例中，我們要根據收件者的語言（法文或英文）建立條件式內容。

1. 開啟傳遞並導覽至「內容編輯」區段。

1. 找到您要新增條件式內容的欄位。 例如，您可以將條件式內容新增至SMS訊息。

1. 按一下欄位旁的&#x200B;**[!UICONTROL 開啟個人化對話方塊]**&#x200B;圖示以開啟運算式編輯器。

   ![](assets/open-perso-editor-sms.png){zoomable="yes"}

1. 在個人化編輯器中，瀏覽至左側的&#x200B;**[!UICONTROL 條件]**&#x200B;功能表。

1. 若要開始建立條件，請按一下&#x200B;**If**&#x200B;函式旁的&#39;+&#39;圖示。 下列行已新增到中央熒幕： `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * 以個人化欄位取代`<FIELD>`，例如收件者的語言： `recipient.language`。
   * 以要滿足的值取代`<VALUE>`。 例如，`'French'`。
   * 以您要顯示給符合指定條件的設定檔的內容取代`Ìnsert content here`。

     ![](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. 指定收件者不符合條件時應顯示的內容。 若要這麼做，請使用&#x200B;**else**&#x200B;協助程式函式：

   1. 將游標放在運算式結束標籤`%>`之前，然後按一下&#x200B;**Else**&#x200B;函式旁的`+`。

   1. 以您要顯示給不符合if函式條件的設定檔的內容取代`Ìnsert content here`。

   ![](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   您也可以使用&#x200B;**else if**&#x200B;協助程式函式來建置具有多個內容變體的條件。 例如，下方的運算式會根據收件者的語言顯示郵件的三種變體：

   ![](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >每次新增協助程式函式時，都會在函式前後自動新增開啟(`<%`)和結束(`%>`)標籤。
   >
   >在運算式中新增「Else」協助程式函式後的範例： >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >請務必移除這些標籤，以避免任何語法錯誤。 在此範例中，移除&#x200B;**else**&#x200B;函式標籤後修正的運算式為：
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. 條件準備就緒後，您可以儲存內容，並透過模擬內容來檢查其呈現。

## 在電子郵件中建立條件式內容 {#condition-condition-builder}

電子郵件中的條件式內容有兩種建立方式：
* 在運算式編輯器中，透過建立包含協助程式函式的條件，
* 在設計電子郵件時可存取的專用條件式內容產生器中。

以下章節提供逐步指示，說明如何使用電子郵件Designer的條件式內容功能建立條件。 有關如何使用運算式編輯器建立條件的詳細資訊，請參閱[這裡](#condition-perso-editor)。

在此範例中，我們要根據收件者的語言建立包含多個變體的電子郵件訊息。 請依照下列步驟操作：

1. 建立或開啟電子郵件傳遞、編輯其內容，然後按一下&#x200B;**[!UICONTROL 編輯電子郵件內文]**&#x200B;按鈕以開啟電子郵件設計工作區。

1. 選取內容元件，然後按一下&#x200B;**[!UICONTROL 啟用條件式內容]**&#x200B;圖示。

   ![](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. **[!UICONTROL 條件式內容]**&#x200B;窗格會在畫面左側開啟。 在此窗格中，您可以使用條件來建立所選內容元件的多個變體。

1. 設定您的第一個變體。 在&#x200B;**[!UICONTROL 條件式內容]**&#x200B;窗格中，將游標暫留在&#x200B;**[!UICONTROL 變體 — 1]**&#x200B;上，然後按一下&#x200B;**[!UICONTROL 新增條件]**&#x200B;按鈕。

   ![](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. 查詢建模器隨即開啟。 它可讓您透過篩選收件者的設定檔資料來建立條件。 [瞭解如何使用查詢模型工具](../query/query-modeler-overview.md)。

   訊息第一個變體的條件就緒後，請按一下&#x200B;**[!UICONTROL 確認]**。 在此範例中，我們將建立以語言為「法文」的收件者為目標的規則。

   ![](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. 該規則現在已關聯至變體。 為了提高可讀性，建議您按一下省略符號選單，重新命名變體。

1. 設定在傳送訊息時符合規則時元件應如何顯示。 在此範例中，如果法文是收件者的慣用語言，我們會想要以法文顯示文字。

   ![](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. 視需要為內容元件新增任意數量的變體。 您可以隨時在變體之間切換，以檢查內容元件將如何根據其條件規則顯示。

   >[!NOTE]
   >如果傳送訊息時不符合變體中所定義的規則，內容元件將會從&#x200B;**[!UICONTROL 條件式內容]**&#x200B;窗格顯示&#x200B;**[!UICONTROL 預設變體]**&#x200B;中所定義的內容。
