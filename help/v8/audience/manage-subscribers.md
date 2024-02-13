---
audience: end-user
title: 管理訂閱者
description: 瞭解如何在Adobe Campaign Web中管理服務並交付給訂閱者
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# 管理訂閱者 {#manage-subscribers}

一旦您 [已建立服務](manage-services.md#create-service)，您可以新增訂閱者、取消訂閱收件者，以及傳送訊息給該服務的訂閱者。

此頁面詳細說明了訂閱者管理。 若要瞭解如何傳送訊息給訂閱者，請參閱 [本節](../msg/send-to-subscribers.md).

## 新增訂閱者至您的服務 {#add-subscribers}

若要手動新增訂閱者，請遵循下列步驟。

1. 從中選擇現有服務 **[!UICONTROL 訂閱服務]** 清單。

1. 前往 **[!UICONTROL 訂閱者]** 標籤並按一下 **[!UICONTROL 新增訂閱者]**.

   ![](assets/service-subscribers-tab.png){zoomable=&quot;yes&quot;}

1. 從清單中選取您要新增的設定檔，然後按一下 **[!UICONTROL 確認]**.

   ![](assets/service-subscribers-select-profiles.png){zoomable=&quot;yes&quot;}

1. 按一下 **[!UICONTROL 傳送]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> 讓選取的收件者接收訂閱 [確認訊息](manage-services.md#create-confirmation-message) 您定義於 [建立服務](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >如果您選取 **[!UICONTROL 取消]**，不會傳送確認訊息給選取的設定檔，但會訂閱設定檔。

新增的設定檔會顯示在 **[!UICONTROL 訂閱者]** 標籤。 他們現在已訂閱您的服務。

## 從您的服務移除訂閱者 {#remove-subscribers}

### 手動取消訂閱收件者 {#manual-unsubscription}

一旦您 [新增的訂閱者](#add-subscribers) 您可手動取消訂閱各項服務。 請遵循下列步驟。

1. 從中選擇現有服務 **[!UICONTROL 訂閱服務]** 清單。

1. 按一下所需收件者名稱旁的三點圖示，然後選取 **[!UICONTROL 刪除]**.

   ![](assets/service-subscribers-delete.png){zoomable=&quot;yes&quot;}

1. 確認刪除。

1. 按一下 **[!UICONTROL 傳送]** 讓選取的收件者收到取消訂閱 [確認訊息](manage-services.md#create-confirmation-message) 您定義於 [建立服務](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png){zoomable=&quot;yes&quot;}

收件者會從 **[!UICONTROL 訂閱者]** 索引標籤上，並已不再訂閱您的服務。

### 自動取消訂閱收件者 {#automatic-unsubscription}

訂閱服務的持續時間有限。 當有效期到期時，收件者會自動取消訂閱。

指定此期間的條件為 [建立服務](manage-services.md#create-service). 從 **[!UICONTROL 其他選項]**，停用 **[!UICONTROL 有效期無限制]** 選項並定義服務的有效期。

![](assets/service-create-validity-period.png){zoomable=&quot;yes&quot;}

指定的期間過期後，所有訂閱者都會自動取消訂閱該服務。
