---
audience: end-user
title: 傳送訊息給服務的訂閱者
description: 瞭解如何傳送訊息給服務的訂閱者
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 傳送訊息給服務的訂閱者 {#send-to-subscribers}

您可以在Adobe Campaign中建立訂閱服務，並傳送訊息給訂閱者。 瞭解如何在[此頁面](../audience//manage-services.md#create-service)上建立訂閱服務。

若要傳送訊息給訂閱者，請建立特定對象來識別訂閱者，然後建立傳送，如下所述。

1. 建立對象。 系統會自動建立新工作流程。 [進一步瞭解對象](../audience/create-audience.md)。

1. 為了更好的可讀性，請在工作流程設定&#x200B;**標籤**&#x200B;欄位中變更工作流程的名稱。 [瞭解如何設定工作流程設定](../workflows/workflow-settings.md)。

1. 開啟&#x200B;**[!UICONTROL 建立對象]**&#x200B;活動，然後選取&#x200B;**[!UICONTROL 建立對象]**。 [瞭解如何設定組建對象活動](../workflows/activities/build-audience.md)。

   ![在Adobe Campaign中顯示「建置對象」活動設定的熒幕擷圖。](assets/service-create-audience.png){zoomable="yes"}

1. 在對象建立流程中，選取下列自訂條件： **[!UICONTROL 訂閱]**&#x200B;存在，例如&#x200B;**[!UICONTROL 服務]**&#x200B;等於您定義的服務。 在此範例中，選取您的&#x200B;**Luma瑜伽電子報**。

   ![熒幕擷圖顯示Adobe Campaign中訂閱之受眾建立流程的自訂條件。](assets/service-audience-subscribers.png){zoomable="yes"}

1. 選取&#x200B;**[!UICONTROL 確認]**，然後按一下&#x200B;**[!UICONTROL 開始]**&#x200B;以執行工作流程。

1. 建立傳遞。 建立傳遞的步驟已詳載於[此頁面](../msg/gs-messages.md#create-delivery)。

1. 瀏覽至您的傳遞設定，並將預設目標對應變更為&#x200B;**訂閱(nms：subscriptions)**。

   ![熒幕擷圖顯示傳遞設定，其中目標對應已變更為Adobe Campaign中的訂閱。](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. 在傳送的主要目標區段中，選取您在上方建立的對象。

   ![熒幕擷圖顯示Adobe Campaign中選定對象之傳遞的主要目標區段。](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. 建立您的訊息內容、測試並傳送傳遞，如[本節](../preview-test/preview-test.md)所詳述。

   ![熒幕擷圖顯示傳遞已準備好在Adobe Campaign中傳送。](assets/service-delivery-ready.png){zoomable="yes"}

您的傳遞只會傳送給該服務的訂閱者。