---
title: '如何製作動態內容？ '
description: 了解如何使用個人化和條件式內容來製作動態內容。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
old-role: Data Architect
role: Developer
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 100%

---

# 如何製作動態內容？  {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="個人化"
>abstract="您可以利用個人化編輯器，選取、排列、自訂和驗證所有資料，為您的內容建立自訂體驗。您可以利用輪廓資料將傳送給各收件者的訊息個人化，以及建立條件式內容，針對每位收件者調整訊息，並僅顯示相關內容。"

身為行銷人員，最重要的事是鎖定真正對產品感興趣的目標客戶，並提供有效且相關的內容與其進行互動。考量到您面對的收件者範圍極為廣泛，若要建立多個行銷內容以吸引不同的人群，可能會既耗時又浪費資源。這種情況正是動態內容發揮重要功用的時候。

您可以使用 Adobe Campaign Web 動態內容功能，根據所收集到關於收件者的資訊來自訂內容。透過動態內容，您可以確保行銷內容更具關聯性，避免行銷不需要或不必要的產品或服務。這種方法使您的內容更具吸引力並增加了讀取內容的可能性。此外，這還能讓您將內容個人化，使收件者感覺他們是在從人而不是機器接收資訊。

## 如何製作動態內容？  {#make-content-dyn}

在 Campaign Web 運算式編輯器中插入 JavaScript 結構，即可製作出動態的訊息內容。傳送訊息時，Adobe Campaign 會解讀這些運算式，將正確的內容傳遞給您的每位收件者：

* 利用每位特定收件者的名字、興趣、居住地、購買的商品等輪廓資料，製作給他們的&#x200B;**個人化訊息**。您可以從個人化編輯器中選取資料庫中與收件者、訊息或傳遞相關的任何可用欄位。您可以將這些個人化屬性插入訊息的主旨行或內文中。以下語法會將收件者的城市插入您的內容中：`<%= recipient.location.city %>`。

  [描述：使用個人化屬性將收件者的城市插入主旨行的範例。](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **建立條件式內容**&#x200B;以針對每個收件者調整傳遞，並僅顯示根據所掌握的客戶資訊和特定客戶相關的內容。這讓您可根據條件顯示特定的文字區塊和/或影像。例如，可根據收件者對特定服務的訂閱調整電子郵件的橫幅。

  [描述：根據收件者的訂閱在電子郵件橫幅中加入條件式內容的範例。](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [在影片中探索此功能](#video)

## 存取運算式編輯器 {#access}

Adobe Campaign Web 會提供運算式編輯器，讓您可以選取、排列、自訂和驗證所有資料，為您的內容打造自訂體驗。您可在所有管道中使用運算式編輯器，在具有&#x200B;**[!UICONTROL 開啟個人化對話框]**&#x200B;圖示的每個欄位中皆可使用，例如主旨行欄位，或電子郵件連結和文字/按鈕內容元件。

以下是關於如何根據要動態化的內容存取運算式編輯器的一些範例：

* *從寄件者姓名欄位存取運算式編輯器*

  [描述：從寄件者姓名欄位存取運算式編輯器的範例。](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *從電子郵件文字元件存取運算式編輯器*

  [描述：從電子郵件文字元件存取運算式編輯器的範例。](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *從電子郵件中的連結存取運算式編輯器*

  [描述：從電子郵件中的連結存取運算式編輯器的範例。](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>除了運算式編輯器之外，設計電子郵件時還可以使用專用的條件式內容建置器。[了解如何在電子郵件中建置條件式內容](conditions.md)

## 操作說明影片 {#video}

了解如何使用運算式編輯器來個人化您的訊息或新增條件內容，藉以製作動態訊息內容。

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)