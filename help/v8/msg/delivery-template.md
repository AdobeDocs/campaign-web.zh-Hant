---
product: campaign
title: 利用傳送範本
description: 瞭解如何在Campaign中建立和使用傳遞範本
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 4a8513bb-8290-432a-8e40-822cd1337cb3
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 3%

---

# 利用傳送範本 {#work-with-delivery-templates}

為了加快並改善設計流程，您可以建立傳遞範本，以在行銷活動中輕鬆重複使用自訂內容。 此功能可讓您標準化創意外觀和風格，以更快執行和啟動行銷活動。

範本可包含：

<!--[Typologies](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html)?
Sender and reply-to addresses?-->
* 一個 [對象](../audience/about-audiences.md)，包括 [控制組](../audience/control-group.md)
* 自訂 [內容](../content/edit-content.md)<!--company logo, or signature-->
* [個人化欄位](../personalization/personalize.md) 和 [條件式內容](../personalization/conditions.md) <!--basic [personalization blocks](../personalization/personalize.md#ootb-content-blocks)-->
* 連結至 [映象頁面](../content/mirror-page.md) 和取消訂閱 [連結](../content/message-tracking.md)

<!--Other delivery properties, such as resource validity, retry parameters, or quarantine settings.-->

## 存取和管理範本 {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="利用傳送範本"
>abstract="使用傳遞範本，輕鬆建立並儲存現有傳遞內容，以供日後使用。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html#copy-an-existing-template" text="複製現有範本"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html#convert-an-existing-delivery" text="將傳遞轉換為範本"

若要存取內容範本清單，請選取 **[!UICONTROL Campaign Management]** > **[!UICONTROL 傳遞]** 從左側功能表，並瀏覽至 **範本** 標籤。

![](assets/templates-tab.png)

所有範本都是 [已建立](#create-a-delivery-template) 隨即顯示於目前環境中。

您可以在頻道和資料夾上篩選內容範本。 您也可以使用傳遞屬性建立規則，以設定進階篩選器。 [進一步瞭解規則產生器](../audience/segment-builder.md)

![](assets/templates-filters.png)

若要編輯範本，請從清單中按一下所需的專案。 從那裡：

* 您可以修改其內容、屬性、對象及附加至該對象的任何選件。
* 您也可以測試範本。 [了解更多](#test-template)

![](assets/templates-edition.png)

若要刪除或 [重複](#copy-an-existing-template) 範本中，選取範本中對應的動作 **[!UICONTROL 更多動作]** 功能表，從 **[!UICONTROL 範本]** 清單或範本版本畫面。

![](assets/templates-more-actions.png)

>[!NOTE]
>
>編輯或刪除範本時，使用此範本建立的傳遞不受影響。

## 建立範本 {#create-a-delivery-template}

若要建立傳遞範本，您可以：
* 複製現有範本 —  [瞭解更多](#copy-an-existing-template)
* 將現有傳遞轉換為範本 —  [瞭解更多](#convert-an-existing-delivery)
* 從頭開始建立傳遞範本 —  [瞭解更多](#create-a-new-template)

### 複製現有範本 {#copy-an-existing-template}

Campaign為每個頻道提供一組內建範本：電子郵件、推播、簡訊。 建立傳遞範本的最簡單方法是複製和自訂內建範本。

>[!NOTE]
>
>您也可以複製任何自訂範本。

若要複製傳遞範本，請遵循下列步驟：

1. 瀏覽至 **範本** 標籤，從 **傳遞** 左側功能表。 [了解更多](#access-manage-templates)
1. 按一下 **[!UICONTROL 更多動作]** 按鈕，然後選取「 」  **[!UICONTROL 複製]**.

   您也可以從清單中選取範本，然後從範本版本畫面中選取此選項。

1. 確認複製。

   ![](assets/templates-duplicate-confirm.png)

1. 新範本控制面板會在中央畫面中開啟。 視需要編輯範本設定。

   ![](assets/templates-duplicated-item.png)

1. 按一下 **[!UICONTROL 檢閱]** 按鈕來儲存及檢閱您的範本。 您仍然可以編輯其所有設定、刪除及複製它。

   ![](assets/templates-review-screen.png)

1. 視需要測試範本呈現。 [了解更多](#test-template)

新範本會新增至 [**範本** 清單](#access-manage-templates). 您現在可以在建立新傳送時選取它。

### 將傳遞轉換為範本 {#convert-an-existing-delivery}

任何傳遞都可以轉換為範本，以供日後重複傳遞動作使用。

若要將傳送儲存為範本，請遵循下列步驟：

1. 前往 **[!UICONTROL 行銷活動管理]** > **[!UICONTROL 傳遞]** 功能表。
1. 從 **[!UICONTROL 瀏覽]** 索引標籤，按一下 **[!UICONTROL 更多動作]** 按鈕，然後選取「 」 **[!UICONTROL 復製為範本]**.

   ![](assets/templates-convert-delivery.png)

1. 確認複製。

1. 新範本控制面板會在中央畫面中開啟。 視需要編輯範本設定。

1. 按一下 **[!UICONTROL 檢閱]** 按鈕來儲存及檢閱您的範本。 您仍然可以編輯其所有設定、刪除及複製它。

1. 視需要測試範本呈現。 [了解更多](#test-template)

新範本會新增至 [**範本** 清單](#access-manage-templates). 您現在可以在建立新傳送時選取它。

### 建立新範本 {#create-a-new-template}

>[!NOTE]
>
>為避免設定錯誤，Adobe建議您 [複製內建範本](#copy-an-existing-template) 並自訂其屬性，而非建立新範本。

若要從頭開始設定傳送範本，請遵循下列步驟：

1. 瀏覽至 **範本** 標籤，從 **傳遞** 左側功能表。 [了解更多](#access-manage-templates)
1. 按一下 **[!UICONTROL 建立範本]** 按鈕。

   ![](assets/templates-create-button.png)

1. 選取您要用於範本的管道。
1. 預設會使用該管道的內建傳遞範本，協助您建立自己的範本。 使用所選管道右側的專用按鈕，視需要選擇其他範本。

   ![](assets/templates-channel-browse.png)

1. 按一下 **[!UICONTROL 建立範本]** 按鈕。

1. 定義範本屬性， [對象](../audience/add-audience.md) 和內容（視選取的頻道而定）。

   >[!NOTE]
   >
   >請在以下章節中進一步瞭解傳遞管道以及如何設計相關內容：
   >
   > * [電子郵件通道](../email/create-email.md)
   > * [推播通知頻道](../push/gs-push.md)
   > * [SMS 頻道](../sms/create-sms.md)


1. 按一下 **[!UICONTROL 檢閱]** 按鈕來儲存及檢閱您的範本。 您仍然可以編輯其所有設定、刪除及複製它。

1. 視需要測試範本呈現。 [了解更多](#test-template)

新範本會新增至 [**範本** 清單](#access-manage-templates). 您現在可以在建立新傳送時選取它。

## 測試傳遞範本 {#test-template}

您可以測試任何傳遞範本的轉譯，無論是從草稿建立還是從現有內容建立。 若要這麼做，請遵循下列步驟。

1. 瀏覽至 **範本** 跳過 **[!UICONTROL 行銷活動管理]** > **[!UICONTROL 傳遞]** 功能表並選取任何範本。 [了解更多](#access-manage-templates)

1. 按一下 **[!UICONTROL 模擬內容]** 按鈕。

   ![](assets/templates-simulate-button.png)

1. 選取一或多個測試設定檔以檢查您的電子郵件呈現。 您也可以從資料庫中選取實際的設定檔。

1. 在不同的設定檔之間切換，以根據選取的設定檔取得訊息的個人化表示。

   <!--[Learn moreon test profiles](../preview-test/proofs.md#recipients)-->

   您也可以調整縮放等級，並選擇案頭或行動檢視。

   ![](assets/templates-stimulate.png)

1. 關閉視窗以返回範本版本畫面。

>[!NOTE]
>
>您不能在傳遞範本中使用電子郵件呈現或傳送校樣。

* [進一步瞭解預覽電子郵件內容](../preview-test/preview-content.md)

* [進一步瞭解預覽SMS內容](../sms/content-sms.md)

* [進一步瞭解預覽推播內容](../push/gs-push.md)

