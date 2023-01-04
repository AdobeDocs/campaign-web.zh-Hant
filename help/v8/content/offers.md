---
audience: end-user
title: 傳送優惠方案
description: 傳送優惠方案
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: bf55b13011f7d2bdafcc55b1b2539c4ce590dd85
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 傳送優惠方案 {#offers-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="選件設定"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="選件進階設定"
>abstract="TBC"

>[!NOTE]
>
>本檔案正在建置中，且經常更新。 此內容的最終版本將於2023年1月推出。

Adobe Campaign v8 web可讓您透過使用 **[!UICONTROL 互動]** 模組。 如需互動以及如何在主控台中管理優惠方案目錄的詳細資訊，請參閱 [Campaign V8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html)

透過電子郵件傳送優惠方案的步驟如下：

1. [設定要建議的選件](#configure),
1. [將優惠方案插入電子郵件](#insert).

## 設定要建議的選件 {#configure}

若要選取要在電子郵件中建議的優惠方案，請按一下 **[!UICONTROL 選件]** 按鈕，然後設定要建議的選件。

![](assets/create-content-offers.png)

1. 選取 **[!UICONTROL 優惠方案空間]** 符合您的優惠方案環境。

1. 若要調整引擎的選件選擇，請選取特定 **[!UICONTROL 選件類別]** 中排序選件。

   若未指定類別，則環境中包含的所有選件將會由選件引擎考慮，除非 **[!UICONTROL 優惠方案主題]** 中所有規則的URL。

   >[!NOTE]
   >
   >主題是類別中上游定義的關鍵字。 它們可作為篩選器，讓您透過在一組類別中選取來調整要顯示的選件數量。

1. 使用 **[!UICONTROL 主張]** 欄位，指定您要插入至電子郵件的優惠方案數量。

1. 選取 **[!UICONTROL 排除不符合資格的收件者]** 選項。

   此選項可讓您啟用或停用排除沒有足夠合格優惠方案的收件者。

   * 如果啟用此選項，則沒有足夠建議的收件者將被排除在傳遞之外。
   * 如果禁用了該選項，則不會排除這些收件者，但他們將沒有請求的數量的建議。

1. 如有必要，請選取 **[!UICONTROL 若未選取選件，則隱藏所有內容]** 選項。

   此選項可讓您選擇在其中一個主張不存在時，如何處理訊息。

   * 如果啟用了該選項，則不會顯示缺少的主張的表示，並且此主張的消息中不會顯示任何內容。
   * 如果禁用該選項，則消息本身在發送期間將被取消，收件者將不再接收任何消息。

將要建議的優惠方案設定到電子郵件後，您就可以使用運算式編輯器將優惠方案插入電子郵件中。 [了解如何將優惠方案插入電子郵件](#insert)

## 將優惠方案插入電子郵件 {#insert}

使用運算式編輯器將選件新增至電子郵件。 可插入下列任一項目：

* 在電子郵件主旨行中，
* 在電子郵件內文中，允許任何內容元件中進行個人化。 [了解如何新增內容元件](content-components.md)

>[!NOTE]
>
>插入優惠方案之前，請確定您已 [設定要透過電子郵件建議哪些優惠方案](#configure).

若要使用運算式編輯器插入選件，請執行下列步驟：

1. 開啟運算式編輯器，然後選取 **[!UICONTROL 主張]** 功能表。

   清單中顯示可用的主張。 在配置要建議的選件時定義命題的數量。

   ![](assets/offer-insertion.png)

1. 使用個人化欄位、呈現函式或提供適用於每個主張的屬性，將主張新增至電子郵件主旨或內文。

   ![](assets/offer-inserted.png)
