---
audience: end-user
title: 管理訂閱者
description: 瞭解如何在Adobe Campaign Web中管理服務並交付給訂閱者
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 管理訂閱者 {#manage-subscribers}

[建立服務](manage-services.md#create-service)之後，您可以新增訂閱者、取消訂閱收件者，以及傳送訊息給該服務的訂閱者。

此頁面詳細說明了訂閱者管理。 若要瞭解如何傳送訊息給訂閱者，請參閱[本節](../msg/send-to-subscribers.md)。

## 新增訂閱者至您的服務 {#add-subscribers}

若要手動新增訂閱者，請遵循下列步驟。

1. 從&#x200B;**[!UICONTROL 訂閱服務]**&#x200B;清單中選取現有的服務。

1. 移至&#x200B;**[!UICONTROL 訂閱者]**&#x200B;索引標籤，然後按一下&#x200B;**[!UICONTROL 新增訂閱者]**。

   ![](assets/service-subscribers-tab.png){zoomable="yes"}

1. 從清單中選取您要新增的設定檔，然後按一下&#x200B;**[!UICONTROL 確認]**。

   ![](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 傳送]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->，讓選取的收件者接收您在[建立服務](manage-services.md#create-service)時所定義的訂閱[確認訊息](manage-services.md#create-confirmation-message)。

   ![](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >如果您選取&#x200B;**[!UICONTROL 取消]**，將不會傳送確認訊息給選取的設定檔，但是它們已訂閱。

新增的設定檔會顯示在&#x200B;**[!UICONTROL 訂閱者]**&#x200B;索引標籤中。 他們現在已訂閱您的服務。

## 從您的服務移除訂閱者 {#remove-subscribers}

### 手動取消訂閱設定檔 {#manual-unsubscription}

一旦您[新增訂閱者](#add-subscribers)至您的服務後，您可以手動取消訂閱每個訂閱者。 請遵循下列步驟。

1. 從&#x200B;**[!UICONTROL 訂閱服務]**&#x200B;清單中選取現有的服務。

1. 按一下所要收件者名稱旁的三點圖示，並選取&#x200B;**[!UICONTROL 刪除]**。

   ![](assets/service-subscribers-delete.png){zoomable="yes"}

1. 確認刪除。

1. 按一下&#x200B;**[!UICONTROL 傳送]**，讓選取的收件者收到您在[建立服務](manage-services.md#create-service)時所定義的取消訂閱[確認訊息](manage-services.md#create-confirmation-message)。

   ![](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

收件者已從&#x200B;**[!UICONTROL 訂閱者]**&#x200B;索引標籤中移除，且不再訂閱您的服務。

### 自動取消訂閱收件者 {#automatic-unsubscription}

訂閱服務的持續時間有限。 當有效期到期時，設定檔會自動取消訂閱。

[建立服務](manage-services.md#create-service)時指定此期間。 從&#x200B;**[!UICONTROL 其他選項]**，停用&#x200B;**[!UICONTROL 無限有效期間]**&#x200B;選項，並定義服務的有效期間。

![](assets/service-create-validity-period.png){zoomable="yes"}

指定的期間過期後，所有訂閱者都會自動取消訂閱該服務。
