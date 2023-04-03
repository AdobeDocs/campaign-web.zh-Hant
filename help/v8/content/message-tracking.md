---
audience: end-user
title: 追蹤您的訊息
description: 了解如何新增連結及追蹤已傳送的訊息
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Infertitive"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# 新增連結及追蹤訊息 {#tracking}

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

所有電子郵件訊息中都應新增鏡像頁面的特定連結。 深入了解鏡像頁面，位於 [本節](mirror-page.md).

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
