---
audience: end-user
title: 追蹤您的訊息
description: 了解如何新增連結和追蹤已傳送的訊息
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 66%

---

# 新增連結和追蹤訊息 {#tracking}

使用電子郵件設計工具將連結新增到內容並追蹤已傳送的訊息以監控收件者的行為。

## 插入連結 {#insert-links}

設計訊息，您可以新增連結到您的內容。

>[!NOTE]
>
>啟用追蹤，將追蹤訊息內容包含的所有連結。

若要將連結插入到電子郵件內容，請依照以下步驟進行：

1. 選取元素，然後從內容關聯式工具列中按一下「**[!UICONTROL 插入連結]**」。

1. 選擇您要建立的連結型別：

   ![](assets/message-tracking-insert-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 外部連結]**：插入外部URL的連結。

     >[!AVAILABILITY]
     >
     >下列功能(連結至 **[!UICONTROL 登陸頁面]**， **[!UICONTROL 訂閱連結]** 和 **[!UICONTROL 取消訂閱連結]**)為有限可用性(LA)。 限製為移轉的客戶 **從Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和無法部署在任何其他環境中。

   * **[!UICONTROL 登陸頁面]**：插入登入頁面的連結。 如果您選取動態登陸頁面(包含 **[!UICONTROL 來自URL的服務]** 選項)，您可以從清單中選取任何服務。 [了解更多](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 訂閱連結]**：插入訂閱服務的連結。 當使用者按一下連結時，系統將他們導向至所選服務中參照的訂閱登入頁面。 [了解更多](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 取消訂閱連結]**：插入取消訂閱服務的連結。 當訂閱者按一下連結時，系統會將他們導向至所選服務中參照的取消訂閱登陸頁面。 [了解更多](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. 在對應欄位中輸入所需的URL，或選取登入頁面或服務，並定義連結設定和樣式。

1. 新增&#x200B;**[!UICONTROL 標籤]**&#x200B;和&#x200B;**[!UICONTROL 連結]**。

1. 儲存您的變更。

1. 建立連結後，您仍然可以從「**[!UICONTROL 設定]**」索引標籤進行修改。

   * 您可以編輯連結並變更其&#x200B;**[!UICONTROL 目標]**。
   * 您可以透過勾選對應的選項來選擇是否為連結加底線。

   ![](assets/message-tracking-link-settings.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>行銷類型電子郵件訊息必須包含選擇退出連結，而異動訊息則不需要。訊息類別(**[!UICONTROL 行銷]** 或 **[!UICONTROL 異動]**)會在頻道介面層級建立訊息時定義。

鏡像頁面的特定連結應新增到您的所有電子郵件訊息。若要了解鏡像頁面的詳細資訊，請參閱[本章節](mirror-page.md)。

## 管理追蹤 {#manage-tracking}

[電子郵件設計工具](create-email-content.md) 可讓您管理被追蹤的 URL，例如編輯每個連結的追蹤類型。

1. 從左窗格按一下「**[!UICONTROL 連結]**」圖示以顯示內容中被追蹤的所有 URL 清單。

   此清單可讓您能夠集中檢視並找到電子郵件內容中的每個 URL。

1. 若要編輯連結，按一下對應的鉛筆圖示。

   ![](assets/message-tracking-edit-links.png){zoomable=&quot;yes&quot;}

1. 您可以修改&#x200B;**[!UICONTROL 追蹤類型]** (如果需要)：

   ![](assets/message-tracking-edit-a-link.png){zoomable=&quot;yes&quot;}

   對於每個被追蹤的 URL，您可以將追蹤模式設定為以下其中一個值：

   * **[!UICONTROL 已追蹤]**：啟動追蹤此 URL。
   * **[!UICONTROL 選擇退出]**：將此 URL 視為選擇退出或取消訂閱 URL。
   * **[!UICONTROL 鏡像頁面]**：將此 URL 視為鏡像頁面 URL。
   * **[!UICONTROL 絕不]**：絕不啟動追蹤此 URL。<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 為您的連結新增&#x200B;**[!UICONTROL 類別]**&#x200B;以將被追蹤的連結群組起來，然後按一下「**[!UICONTROL 儲存]**」。

   ![](assets/message-tracking-edit-a-link_2.png){zoomable=&quot;yes&quot;}

1. 傳送您的傳遞後，存取傳遞報告。在「**[!UICONTROL 追蹤]**」選單下，**[!UICONTROL URL 和點按資料流]** 報告顯示您的傳遞中哪些 URL 造訪次數最多。[了解更多](../reporting/gs-reports.md)
