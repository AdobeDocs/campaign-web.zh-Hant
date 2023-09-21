---
audience: end-user
title: 在您的訊息中新增優惠方案
description: 瞭解如何新增及傳送優惠方案
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 33%

---


# 在您的訊息中新增優惠方案 {#offers-content}

Adobe Campaign v8網頁版可讓您使用在主控台中建立的傳送選件，連同傳送給使用者。 **[!UICONTROL 互動]** 模組。 如需互動以及如何管理主控台中的優惠方案目錄的詳細資訊，請參閱 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

透過傳送傳送優惠方案的步驟如下：

1. [設定要提出的優惠](#configure)
1. [將優惠方案插入傳遞](#insert)

## 設定要提出的優惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="定義優惠引數"
>abstract="透過定義優惠空間（可選擇類別和主題），設定應向收件者建議的優惠，並指定要插入傳遞中的優惠方案數量。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="設定優惠方案進階設定"
>abstract="您可以啟用排除沒有足夠合格優惠的收件者，並選擇當其中一個主張不存在時如何處理訊息。"

Adobe Campaign可讓您向指定連絡人建議一或多個特定優惠方案。 互動模組，可讓您在互動期間透過建議單一或數個特定優惠方案，即時回應指定的聯絡人。 這些優惠方案可以是簡單的通訊訊息、一或多個產品或服務的特別優惠方案。

若要選取要新增至傳送的優惠方案，請遵循下列步驟。

1. 按一下 **[!UICONTROL 設定優惠方案]** 傳遞內容版本畫面中的按鈕。

   ![](assets/setup-offers.png)

1. 設定應向收件者提出的優惠。

   首先選取與您的優惠環境相符的&#x200B;**[!UICONTROL 優惠空間]**。瞭解如何在中建立優惠空間 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}

   ![](assets/create-content-offers.png)

1. 若要縮小引擎的優惠選擇範圍，請選取特定的&#x200B;**[!UICONTROL 優惠類別]**，優惠在此類別中排序。

   選取資料夾時，會自動包含所有子資料夾，且無法移除。 請注意 [!DNL Campaign] 介面不會反映此行為。

   >[!NOTE]
   >
   >如果未指定類別，則優惠引擎會將環境包含的所有優惠考慮在內，除非有選取&#x200B;**[!UICONTROL 優惠主題]**。

1. （選擇性）輸入主題以篩選類別。 主題是在類別上游定義的關鍵詞。主題做為篩選器，在一組類別中選擇主題即可讓您調整要顯示的優惠數量。

1. 使用 **[!UICONTROL 主張]** 欄位，指定您要插入傳遞中的選件數量。

1. 選取「**[!UICONTROL 排除不符合資格的收件者]**」選項 (如有必要)。

   此選項可讓您啟用或停用排除收件者，這些收件者沒有足夠符合資格優惠可提供給他們。

   * 如果啟用該選項，則沒有足夠提議的收件者被排除在傳遞作業之外。
   * 如果該選項停用，這些收件者不會被排除在外，但他們不能擁有要求的提議數量。

1. 如有必要，選取「**[!UICONTROL 如果未選取任何優惠，則隱藏所有內容]**」選項。

   此選項可讓您選擇其中一個提議不存在時要如何處理訊息。

   * 如果啟用該選項，則不會顯示遺失的提議，且此提議的內容不會出現在訊息中。
   * 如果停用該選項，訊息本身在傳送期間會被取消，收件者無法再收到任何訊息。

將優惠方案設定為建議至您的傳送後，您可以使用運算式編輯器將其插入傳送內容。

## 將優惠插入傳遞 {#insert}

可使用將優惠新增至傳遞中 [運算式編輯器](../personalization/gs-personalization.md#access). 它們可以插入主旨行或傳遞內文中。

>[!CAUTION]
>
>將選件插入傳遞之前，請確定您已 [已設定要與該傳送一起建議哪些優惠](#configure).

若要使用運算式編輯器插入選件，請遵循下列步驟。

1. 存取主旨列或任何傳遞的內容。

1. 將滑鼠游標置於您要插入選件的位置，並使用個人化圖示開啟運算式編輯器。

1. 選取 **[!UICONTROL 主張]** 功能表。 可用的提議會顯示在清單中。

   >[!NOTE]
   >
   >在以下情況下會定義主張數量： [設定優惠方案](#configure) 用於目前的傳遞。

   ![](assets/offer-insertion.png)

1. 使用個人化欄位、呈現函式或每個主張可用的優惠方案屬性，將主張新增至傳遞主題行或內文。

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >可用的主張數量取決於引擎呼叫的設定方式，而其順序則取決於優惠方案的優先順序。 進一步瞭解 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. 儲存您的變更。

1. 完成內容、測試並傳送您的傳遞。

現在，當收件者收到傳遞時，正確的優惠方案會顯示給該特定設定檔。
