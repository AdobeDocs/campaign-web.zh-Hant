---
title: '如何製作動態內容？ '
description: 了解如何使用個人化和條件式內容來製作動態內容。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 47%

---

# 如何製作動態內容？  {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="個人化"
>abstract="個人化編輯器可讓您選取、排列、自訂和驗證所有資料，為您的內容建立自訂體驗。 您可以利用輪廓資料將傳送每個收件者的訊息個人化，並建立條件式內容，針對每個收件者調整訊息，並僅顯示相關內容。"

身為行銷人員，鎖定對您的產品真正感興趣的客戶，並透過提供有效且相關的內容來吸引他們，是很重要的事。 考慮到您面對的收件者範圍極為廣泛，若要建立多個行銷內容以訴求不同的人群可能既費時又浪費資源。這就是動態內容變得不可或缺的地方。

Adobe Campaign網路動態內容功能可讓您根據所收集關於收件者的資訊來自訂內容。 使用動態內容可確保行銷工作更具相關性，避免行銷不需要或不必要的產品或服務。 這種方法使您的內容更具吸引力並增加了讀取內容的可能性。此外，這還能讓您將內容個人化，使收件者感覺他們是在從人而不是機器接收資訊。

## 如何製作動態內容？  {#make-content-dyn}

您可以在Campaign網頁運算式編輯器中插入JavaScript建構，讓訊息內容呈現動態變化。 在傳送訊息時，Adobe Campaign會解譯這些運算式，以將正確的內容傳遞給每個收件者：

* 利用每個特定收件者的名字、興趣、居住地、購買的商品等輪廓資料傳送&#x200B;**個人化訊息**&#x200B;給他們。您可以從與收件者、訊息或傳遞相關的個人化編輯器中，選取資料庫中可用的任何欄位。 可將這些個人化屬性插入訊息的主旨行或內文中。下列語法在您的內容中插入收件者的城市： `<%= recipient.location.city %>`。

  [說明：使用個人化屬性將收件者的城市插入主旨行的範例。](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **建立條件式內容**&#x200B;以針對每個收件者調整傳遞，並僅顯示根據所掌握的客戶資訊和特定客戶相關的內容。這讓您可根據條件顯示特定的文字區塊和/或影像。例如，可根據收件者對特定服務的訂閱調整電子郵件的橫幅。

  [說明：根據收件者訂閱的電子郵件橫幅的條件式內容範例。](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [在影片中探索此功能](#video)

## 存取運算式編輯器 {#access}

Adobe Campaign Web提供運算式編輯器，您可在其中選取、排列、自訂及驗證所有資料，以建立內容的自訂體驗。 運算式編輯器可用於所有管道，在每個具有&#x200B;**[!UICONTROL 開啟個人化對話方塊]**&#x200B;圖示的欄位中，例如主旨行欄位，或電子郵件連結和文字/按鈕內容元件。

以下是如何根據您要建立動態的內容來存取運算式編輯器的部分範例：

* *從寄件者姓名欄位存取運算式編輯器*

  [描述：從[寄件者名稱]欄位存取運算式編輯器的範例。](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *從電子郵件文字元件存取運算式編輯器*

  [說明：從電子郵件文字元件存取運算式編輯器的範例。](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *從電子郵件中的連結存取運算式編輯器*

  [說明：從電子郵件中的連結存取運算式編輯器的範例。](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>除了運算式編輯器之外，在設計電子郵件時，您也可以使用專用的條件式內容產生器。 [了解如何在電子郵件中建置條件式內容](conditions.md)

## 操作說明影片 {#video}

了解如何使用運算式編輯器來個人化您的訊息或新增條件內容，藉以製作動態訊息內容。

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)