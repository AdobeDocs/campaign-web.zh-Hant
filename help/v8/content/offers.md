---
audience: end-user
title: 傳送優惠
description: 傳送優惠
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: 9203d2bcfbe75b584ecab65637b5ded202435d29
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 47%

---


# 傳送優惠 {#offers-content}

Adobe Campaign v8網頁版可讓您使用在主控台中建立的傳送選件，連同傳送給使用者。 **[!UICONTROL 互動]** 模組。 如需互動及如何在主控台管理優惠目錄的詳細資訊，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}。

透過傳送傳送優惠方案的步驟如下：

1. [設定要提出的優惠](#configure)
1. [將優惠方案插入傳遞中](#insert)

## 設定要提出的優惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="優惠設定"
>abstract="設定應向收件者提出的優惠。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="提供進階設定"
>abstract="設定優惠進階選項。"

1. 若要選取要在傳送中建議的優惠方案，請按一下 **[!UICONTROL 設定優惠方案]** 按鈕（從「傳遞內容版本」畫面）。

   ![](assets/setup-offers.png)

1. 設定應向收件者提出的優惠。

   首先選取與您的優惠環境相符的&#x200B;**[!UICONTROL 優惠空間]**。瞭解如何在中建立優惠空間 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}

   ![](assets/create-content-offers.png)

1. 若要縮小引擎的優惠選擇範圍，請選取特定的&#x200B;**[!UICONTROL 優惠類別]**，優惠在此類別中排序。

   選取資料夾時，會自動包含所有子資料夾，且無法移除。 請注意 [!DNL Campaign] 介面不會反映此行為。

   >[!NOTE]
   >
   >如果未指定類別，則優惠引擎會將環境包含的所有優惠考慮在內，除非有選取&#x200B;**[!UICONTROL 優惠主題]**。

1. （選用）輸入主題以篩選類別。 主題是在類別上游定義的關鍵詞。主題做為篩選器，在一組類別中選擇主題即可讓您調整要顯示的優惠數量。

1. 使用 **[!UICONTROL 主張]** 欄位，指定您要插入傳遞中的優惠方案數量。

1. 選取「**[!UICONTROL 排除不符合資格的收件者]**」選項 (如有必要)。

   此選項可讓您啟用或停用排除收件者，這些收件者沒有足夠符合資格優惠可提供給他們。

   * 如果啟用該選項，則沒有足夠提議的收件者被排除在傳遞作業之外。
   * 如果該選項停用，這些收件者不會被排除在外，但他們不能擁有要求的提議數量。

1. 如有必要，選取「**[!UICONTROL 如果未選取任何優惠，則隱藏所有內容]**」選項。

   此選項可讓您選擇其中一個提議不存在時要如何處理訊息。

   * 如果啟用該選項，則不會顯示遺失的提議，且此提議的內容不會出現在訊息中。
   * 如果停用該選項，訊息本身在傳送期間會被取消，收件者無法再收到任何訊息。

將優惠方案設定為建議至傳遞後，您可以使用運算式編輯器將其插入傳遞內容。

## 將優惠插入傳遞 {#insert}

可使用將優惠方案新增至傳遞中 [運算式編輯器](../personalization/gs-personalization.md#access). 它們可以插入主旨行或傳遞內文中。

>[!CAUTION]
>
>將優惠方案插入傳遞之前，請確定您已 [已設定要與該傳送一起建議哪些優惠](#configure).

若要使用運算式編輯器插入選件，請遵循下列步驟。

1. 存取任何傳遞的主題行或內容。

1. 將滑鼠游標放在您要插入選件的位置，並使用個人化圖示開啟運算式編輯器。

1. 選取 **[!UICONTROL 主張]** 功能表。 可用的提議會顯示在清單中。

   >[!NOTE]
   >
   >在以下情況下，會定義主張數量： [設定優惠方案](#configure) 用於目前的傳遞。

   ![](assets/offer-insertion.png)

1. 使用每個主張可用的個人化欄位、演算函式或優惠方案屬性，將主張新增至傳遞主題行或內文。

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >可用主張的數量取決於引擎呼叫的設定方式，而其順序則取決於優惠方案的優先順序。

1. 儲存您的變更。

1. 完成內容、測試並傳送您的傳遞。

現在，當收件者收到傳遞時，將會對該特定設定檔顯示正確的優惠。
