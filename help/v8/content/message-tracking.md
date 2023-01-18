---
audience: end-user
title: 追蹤您的訊息
description: 了解如何新增連結及追蹤已傳送的訊息
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# 新增連結及追蹤訊息 {#tracking}

![](../assets/do-not-localize/badge.png)

使用電子郵件設計工具來新增內容的連結並追蹤傳送的訊息，以監控收件者的行為。

## 插入連結 {#insert-links}

設計訊息時，您可以新增連結至內容。

>[!NOTE]
>
>啟用追蹤時，會追蹤包含在訊息內容中的所有連結。

若要將連結插入電子郵件內容，請遵循下列步驟：

1. 選取元素並按一下 **[!UICONTROL 插入連結]** 中。

   ![](assets/message-tracking-insert-link.png)

1. 新增 **[!UICONTROL 標籤]** 和 **[!UICONTROL 連結]**.

1. 儲存您的變更。

1. 建立連結後，您仍可從 **[!UICONTROL 元件設定]** 窗格。

   * 您可以編輯連結並變更其 **[!UICONTROL 目標]**.
   * 您可以核取對應的選項，選擇是否將連結加底線。

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>行銷類型的電子郵件訊息必須包含選擇退出連結，這對於交易式訊息並非必要。 訊息類別(**[!UICONTROL 行銷]** 或 **[!UICONTROL 交易]**)是在通道表面（即訊息預設集）層級和建立訊息時定義。

## 連結至鏡像頁面 {#mirror-page}

鏡像頁面是可透過網頁瀏覽器線上存取的HTML頁面。 其內容與您的電子郵件內容相同。

若要將連結新增至電子郵件中的鏡像頁面：

1. 選取元素並按一下 **[!UICONTROL 插入連結]** 中。

   ![](assets/message-tracking-mirror-page.png)

1. 選取 **[!UICONTROL 插入連結]** 圖示來存取個人化功能表。

   ![](assets/message-tracking-mirror-page_2.png)

1. 從 **[!UICONTROL 內容區塊]** 菜單，選擇 **[!UICONTROL 鏡像頁面URL]** 按一下 **[!UICONTROL 新增]**.

   ![](assets/message-tracking-mirror-page_3.png)

鏡像頁面會自動建立。

>[!IMPORTANT]
>
>鏡像頁面連結會自動產生，且無法編輯。 它們包含呈現原始電子郵件所需的所有加密個人化資料。 因此，使用具有大值的個人化屬性可能會產生長的鏡像頁面URL，而這會使連結無法在URL長度上限的網頁瀏覽器中運作。

傳送電子郵件後，當收件者按一下鏡像頁面連結時，電子郵件的內容會顯示在其預設的網頁瀏覽器中。

>[!NOTE]
>
>在傳送至測試設定檔的測試電子郵件中，鏡像頁面的連結未作用中。 它只會在最終訊息中啟動。

鏡像頁面的保留期為60天。 延遲後，鏡像頁面將不再可用。

## 管理追蹤 {#manage-tracking}

此 [電子郵件設計工具](create-email-content.md) 可讓您管理追蹤的URL，例如編輯每個連結的追蹤類型。

1. 按一下 **[!UICONTROL 連結]** 圖示，顯示要追蹤之內容的所有URL清單。

   此清單可讓您集中檢視，並找出電子郵件內容中的每個URL。

1. 若要編輯連結，請按一下對應的鉛筆圖示。

   ![](assets/message-tracking-edit-links.png)

1. 您可以修改 **[!UICONTROL 追蹤類型]** 如有需要：

   ![](assets/message-tracking-edit-a-link.png)

   對於每個追蹤的URL，您可以將追蹤模式設為下列其中一個值：

   * **[!UICONTROL 追蹤]**:在此URL上啟用追蹤。
   * **[!UICONTROL 選擇退出]**:將此URL視為選擇退出或取消訂閱URL。
   * **[!UICONTROL 鏡像頁面]**:將此URL視為鏡像頁面URL。
   * **[!UICONTROL 從不]**:切勿啟用此URL的追蹤。 <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 新增 **[!UICONTROL 類別]** 連結至群組追蹤的連結，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. 傳送您的傳送後，請存取您的傳送報表。 在 **[!UICONTROL 追蹤]** , **[!UICONTROL URL和點按資料流]** 報表會顯示您傳送中最常造訪的URL。 [了解更多](../reporting/reports.md)
