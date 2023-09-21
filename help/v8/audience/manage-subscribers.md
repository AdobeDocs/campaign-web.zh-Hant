---
audience: end-user
title: 管理服務的訂閱者
description: 瞭解如何在Adobe Campaign Web中管理服務並交付給訂閱者
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# 管理服務的訂閱者 {#manage-subscribers}

一旦您 [已建立服務](manage-services.md#create-service)，您可以新增訂閱者、取消訂閱收件者，以及傳送訊息給該服務的訂閱者。

此頁面詳細說明了訂閱者管理。 若要瞭解如何傳送訊息給訂閱者，請參閱 [本節](../content/send-to-subscribers.md).

## 新增訂閱者至您的服務 {#add-subscribers}

若要手動新增訂閱者，請遵循下列步驟。

1. 從中選擇現有服務 **[!UICONTROL 訂閱服務]** 清單。

1. 選取 **[!UICONTROL 訂閱者]** 標籤並按一下 **[!UICONTROL 新增設定檔]**.

   ![](assets/service-subscribers-tab.png)

1. 從清單中選取您要新增的設定檔，然後按一下 **[!UICONTROL 確認]**.

   ![](assets/service-subscribers-select-profiles.png)

1. 按一下 **[!UICONTROL 傳送]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> 選取的收件者將收到訂閱 [確認訊息](manage-services.md#create-confirmation-message) 您選擇的時機 [建立服務](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

新增的設定檔會顯示在 **[!UICONTROL 訂閱者]** 清單。 他們現在已訂閱您的服務。

## 從您的服務移除訂閱者 {#remove-subscribers}

### 手動取消訂閱收件者 {#manual-unsubscription}

一旦您 [新增的訂閱者](#add-subscribers) 您可手動取消訂閱各項服務。 請遵循下列步驟。

1. 從中選擇現有服務 **[!UICONTROL 訂閱服務]** 清單。

1. 按一下所需收件者名稱旁的三點圖示，然後選取 **[!UICONTROL 刪除]**.

   ![](assets/service-subscribers-delete.png)

1. 確認刪除並按一下 **[!UICONTROL 傳送]**. 選取的收件者將收到取消訂閱 [確認訊息](manage-services.md#create-confirmation-message) 您選擇的時機 [建立服務](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

收件者會從 **[!UICONTROL 訂閱者]** 清單且不再訂閱您的服務。

### 自動取消訂閱收件者 {#automatic-unsubscription}

訂閱服務的持續時間有限。 當有效期到期時，收件者會自動取消訂閱。

指定此期間的條件為 [建立服務](manage-services.md#create-service). 從 **[!UICONTROL 其他選項]**，停用 **[!UICONTROL 有效期無限制]** 選項並定義服務的有效期。

![](assets/service-create-validity-period.png)

指定的期間過期後，所有訂閱者都會自動取消訂閱該服務。
