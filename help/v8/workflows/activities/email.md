---
audience: end-user
title: 使用電子郵件工作流程活動
description: 瞭解如何使用電子郵件工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: caa994a1f390248c9fe11da198ab73197b129263
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 電子郵件、簡訊、推播 {#channel}

Adobe Campaign Web可讓您跨多個管道（例如電子郵件、簡訊或推播）自動執行行銷活動。 您可以將管道活動結合到畫布中，以建立跨管道工作流程，其可根據客戶行為觸發動作。

例如，您可以建立一個歡迎電子郵件活動，其中包括跨不同管道的一系列訊息，例如電子郵件、簡訊和推播。您還可以在客戶完成購買後傳送後續追蹤電子郵件，或透過簡訊向客戶傳送個人化的生日祝賀訊息。

透過使用管道活動，您可以建立全面且個人化的行銷活動，吸引多個接觸點的客戶並促進轉換。

以下是新增 **頻道** 工作流程中的活動：

1. 確定您已新增 **建立對象** 活動。 對象是傳遞的主要目標：接收訊息的收件者。 在行銷活動工作流程的內容中傳送訊息時，訊息對象不會定義在管道活動中，而是定義在 **建立對象** 活動。 請參閱[本節](build-audience.md)。

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 選取傳遞活動：**[!UICONTROL 電子郵件]**、**[!UICONTROL 簡訊]**、**[!UICONTROL 推播通知 (Android)]** 或&#x200B;**[!UICONTROL 推播通知 (iOS)]**。

1. 選取 **範本**. 範本是預先設定的傳遞設定，儲存供未來使用。[了解更多](../../msg/delivery-template.md)

1. 按一下 **建立傳遞** 和定義訊息的方式，與建立獨立傳送的方式相同。 這也是您定義傳送設定、排程和模擬內容的地方。 [了解更多](../../msg/gs-messages.md)

1. 導覽回您的工作流程，然後按一下 **開始** 以啟動工作流程。

   依預設，啟動傳遞工作流程會觸發訊息準備階段，而不會立即傳送訊息。

1. 按一下 **檢閱並傳送** ，以確認傳送。

1. 從您的傳送控制面板，按一下 **傳送**.

## 範例

以下是跨管道工作流程範例，其中包含細分和兩個傳送。 工作流程會鎖定擁有電子郵件地址並對咖啡機感興趣的所有客戶。 在此群體中，會傳送電子郵件給一般客戶，並傳送簡訊給VIP使用者端。

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

電子郵件收件者會透過對象目標活動在同一工作流程中的活動上游定義。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
