---
audience: end-user
title: 傳送優惠
description: 傳送優惠
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 100%

---


# 傳送優惠 {#offers-content}

Adobe Campaign v8 Web 允許您使用&#x200B;**[!UICONTROL 互動]**&#x200B;模組傳送在主控台中建立的電子郵件優惠。如需互動及如何在主控台管理優惠目錄的詳細資訊，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}。

使用電子郵件傳送優惠的步驟如下所示：

1. [設定要提出的優惠](#configure)，
1. [將優惠插入電子郵件](#insert)。

## 設定要提出的優惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="優惠設定"
>abstract="設定應向收件者提出的優惠。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="優惠進階設定"
>abstract="設定優惠進階選項。"

1. 若要選取要在您的電子郵件中提出的優惠，請從電子郵件內容版本畫面按一下「**[!UICONTROL 優惠]**」按鈕。

   ![](assets/setup-offers.png)

1. 設定應向收件者提出的優惠。首先選取與您的優惠環境相符的&#x200B;**[!UICONTROL 優惠空間]**。

   ![](assets/create-content-offers.png)

1. 若要縮小引擎的優惠選擇範圍，請選取特定的&#x200B;**[!UICONTROL 優惠類別]**，優惠在此類別中排序。

   如果未指定類別，則優惠引擎會將環境包含的所有優惠考慮在內，除非有選取&#x200B;**[!UICONTROL 優惠主題]**。

   >[!NOTE]
   >
   >主題是在類別上游定義的關鍵詞。主題做為篩選器，在一組類別中選擇主題即可讓您調整要顯示的優惠數量。

1. 使用&#x200B;**[!UICONTROL 提議]**&#x200B;欄位可指定要插入電子郵件的優惠數量。

1. 選取「**[!UICONTROL 排除不符合資格的收件者]**」選項 (如有必要)。

   此選項可讓您啟用或停用排除收件者，這些收件者沒有足夠符合資格優惠可提供給他們。

   * 如果啟用該選項，則沒有足夠提議的收件者被排除在傳遞作業之外。
   * 如果該選項停用，這些收件者不會被排除在外，但他們不能擁有要求的提議數量。

1. 如有必要，選取「**[!UICONTROL 如果未選取任何優惠，則隱藏所有內容]**」選項。

   此選項可讓您選擇其中一個提議不存在時要如何處理訊息。

   * 如果啟用該選項，則不會顯示遺失的提議，且此提議的內容不會出現在訊息中。
   * 如果停用該選項，訊息本身在傳送期間會被取消，收件者無法再收到任何訊息。

設定要在電子郵件中提出的優惠後，您可以使用運算式編輯器將它們插入電子郵件中。[了解如何將優惠插入電子郵件](#insert)

## 將優惠插入電子郵件 {#insert}

可以使用運算式編輯器將優惠新增到電子郵件中。優惠可以插入到：

* 電子郵件的主旨行或
* 電子郵件內文，方式是允許在任何內容元件進行個人化。[了解如何新增內容元件](content-components.md)

>[!NOTE]
>
>在插入優惠之前，請確保您已[設定要在電子郵件中提出的優惠](#configure)。

若要使用運算式編輯器插入優惠，請依照以下步驟操作：

1. 開啟運算式編輯器，然後選取「**[!UICONTROL 提議]**」選單。

   可用的提議會顯示在清單中。提議的數量是在設定要提出的優惠時定義的。

   ![](assets/offer-insertion.png)

1. 使用個人化欄位、轉譯功能或每個提議可用的優惠屬性，將提議新增到電子郵件主旨或內文。

   ![](assets/offer-inserted.png)
