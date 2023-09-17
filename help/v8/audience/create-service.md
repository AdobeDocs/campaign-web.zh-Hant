---
audience: end-user
title: 使用訂閱服務
description: 瞭解如何在Adobe Campaign Web中建立服務
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# 使用訂閱服務 {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="建立並管理您的服務"
>abstract="使用Adobe Campaign建立及監控您的服務（例如電子報），並檢查這些服務的訂閱/取消訂閱。 訂閱僅適用於電子郵件和簡訊傳遞。"

使用Adobe Campaign網頁管理及建立您的服務（例如電子報），並檢查這些服務的訂閱/取消訂閱。

>[!NOTE]
>
>訂閱僅適用於電子郵件和簡訊傳遞。

數個服務可並行定義，例如：特定產品類別、網站主題或區域的電子報、各種警報訊息型別的訂閱以及即時通知。

若要進一步瞭解管理訂閱和取消訂閱，請參閱 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## 存取訂閱服務 {#access-services}

若要存取您的平台所提供的訂閱服務，請瀏覽至 **[!UICONTROL 訂閱服務]** 功能表位於左側導覽邊欄中。

![](assets/service-list.png)

此時會顯示所有現有訂閱服務的清單。 您可以搜尋服務並在頻道、資料夾上篩選，或使用進階篩選。

![](assets/service-filters.png)

若要編輯現有服務，請按一下其名稱。

## 建立您的第一個訂閱服務 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="訂閱服務屬性"
>abstract="輸入訂閱服務的標籤，並定義其他選項。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="訂閱服務確認訊息"
>abstract="當使用者訂閱服務或取消訂閱服務時，您可以傳送確認訊息。 選取要用於這些訊息的範本。"


若要建立訂閱服務，請遵循下列步驟：

1. 選取 **[!UICONTROL 建立訂閱服務]** 按鈕。

   ![](assets/service-create-button.png)

1. 選取頻道： **[!UICONTROL 電子郵件]** 或 **[!UICONTROL 簡訊]**.

1. 在服務屬性中，輸入標籤，並視需要定義其他選項。

   ![](assets/service-create-properties.png)

1. 依預設，訂閱沒有限制。 您可以停用 **[!UICONTROL 有效期無限制]** 定義服務有效持續時間的選項。 <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. 當使用者訂閱或取消訂閱服務時，您可以傳送確認訊息。 根據您的使用案例，選取要用於該訊息的範本。

   ![](assets/service-create-confirmation-msg.png)

1. 按一下「**[!UICONTROL 儲存]**」。新服務將新增至 **[!UICONTROL 訂閱服務]** 清單。

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


