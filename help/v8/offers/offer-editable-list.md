---
audience: end-user
title: 將可編輯清單新增至選件結構描述
description: 瞭解如何直接在優惠方案詳細資訊畫面中將自訂集合連結顯示為可編輯的清單。
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 1%

---

# 將可編輯清單新增至選件結構描述 {#offer-editable-list}

當您使用自訂集合連結（例如連結至優惠方案的一組區段）來[擴充 [!DNL nms:offer] 結構描述](../administration/schemas.md)時，可以直接在優惠方案的&#x200B;**[!UICONTROL 自訂選項]**&#x200B;區段中將其顯示為可編輯清單。 集合不會透過個別畫面管理相關記錄，而是呈現為優惠詳細資料中的清單，您可以透過專用對話方塊內嵌建立新的相關記錄。

>[!NOTE]
>
>此功能目前僅適用於優惠方案結構描述。

## 新增集合連結欄位 {#add-field}

1. 使用您的自訂集合擴充[!DNL nms:offer]結構描述，然後瀏覽至&#x200B;**[!UICONTROL 結構描述]**&#x200B;功能表、開啟&#x200B;**[!UICONTROL 行銷優惠方案]**&#x200B;結構描述，然後按一下&#x200B;**[!UICONTROL 熒幕版本]**。 [了解更多資訊](../administration/schemas-browse-access.md#screen-def)。

   ![熒幕擷圖顯示熒幕定義按鈕。](assets/offers-editable-list.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 詳細畫面組態]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL 自訂欄位清單]**&#x200B;表格上方的省略符號圖示，然後選擇&#x200B;**[!UICONTROL 選取屬性]**。 [了解更多資訊](../administration/schemas-custom-fields.md)。

   ![熒幕擷圖顯示熒幕定義按鈕。](assets/offers-editable-list-0.png){zoomable="yes"}

1. 瀏覽屬性並選取您的自訂集合連結，由其集合圖示識別。

   ![熒幕擷圖顯示具有集合連結屬性的屬性選擇器。](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >集合連結欄位無法設為強制欄位，且不支援子屬性。 依預設，它們會跨越表單中的兩欄。

1. 確認您的選取。 集合連結已新增至自訂欄位&#x200B;**資料表的**&#x200B;清單，並以&#x200B;**[!UICONTROL 集合]**&#x200B;作為其型別。

   ![熒幕擷圖顯示新增的屬性。](assets/offers-editable-list-2.png){zoomable="yes"}

## 設定集合的可編輯清單 {#configure-list}

1. 按一下集合欄位列上的省略符號圖示，然後選擇&#x200B;**[!UICONTROL 編輯]**&#x200B;以開啟&#x200B;**[!UICONTROL 集合連結設定]**&#x200B;對話方塊。

   ![顯示編輯按鈕的熒幕擷圖。](assets/offers-editable-list-3.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 一般]**&#x200B;索引標籤中，選擇性地設定&#x200B;**[!UICONTROL Visible if]**&#x200B;條件，或啟用&#x200B;**[!UICONTROL 唯讀]**。

   ![顯示版本熒幕的熒幕擷圖。](assets/offers-editable-list-4.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 熒幕組態]**&#x200B;索引標籤中，按一下&#x200B;**[!UICONTROL 選取屬性]**，並選取將新元素新增至清單時要使用的屬性，例如區段名稱和自訂欄位。

   ![熒幕擷圖顯示集合連結設定對話方塊的熒幕設定索引標籤。](assets/offers-editable-list-5.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 配置]**&#x200B;索引標籤中，保留或清除&#x200B;**[!UICONTROL 跨越兩欄]**。

1. 按一下&#x200B;**[!UICONTROL 確認]**，然後&#x200B;**[!UICONTROL 儲存]**&#x200B;熒幕定義。

## 在選件中使用可編輯清單 {#use-list}

1. 從左側功能表，按一下&#x200B;**選件**&#x200B;並開啟選件。 [閱讀更多](create-offer.md#create)

   ![顯示優惠方案熒幕的熒幕擷圖。](assets/offers-editable-list-7.png){zoomable="yes"}

1. 存取優惠屬性。 集合在&#x200B;**自訂選項**&#x200B;區段中呈現為清單。

   ![在選件詳細資訊畫面中顯示可編輯清單演算的熒幕擷圖。](assets/offers-editable-list-6.png){zoomable="yes"}

1. 按一下[新增]&#x200B;**&#x200B;**&#x200B;以顯示您設定的屬性，填入這些屬性，然後按一下[確認]&#x200B;**&#x200B;**。 新元素會新增至清單中。

   您可以將多個元素新增至相同清單，而選件詳細資料可包含多個可編輯清單。

1. 按一下「**[!UICONTROL 儲存]**」。

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->