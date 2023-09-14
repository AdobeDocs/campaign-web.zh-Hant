---
audience: end-user
title: 使用傳遞工作流程活動
description: 了解如何新增傳遞工作流程活動 (電子郵件、推播、簡訊)
badge: label="Beta"
source-git-commit: 207328a32ba74159d555616f046240100787f20e
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 78%

---


# 電子郵件、簡訊、推播活動 {#channel}

Adobe Campaign Web 讓您能夠跨電子郵件、簡訊和推播管道自動執行行銷活動。您可以將管道活動組合到工作流程畫布中，建立可根據客戶行為和資料觸發動作的跨管道工作流程。

例如，您可以建立一個歡迎電子郵件活動，其中包括跨不同管道的一系列訊息，例如電子郵件、簡訊和推播。您還可以在客戶完成購買後傳送後續追蹤電子郵件，或透過簡訊向客戶傳送個人化的生日祝賀訊息。

使用管道活動，您即可建立全面性和個人化的行銷活動，從多個接觸點和客戶互動並提升轉換率。

>[!NOTE]
>
>您也可以在行銷活動工作流程的內容之外建立單次傳送。 請在以下章節瞭解更多資訊：
>* [建立獨立的電子郵件傳遞](../../email/create-email.md
>* [建立獨立簡訊傳遞](../../sms/create-sms.md)
>* [建立獨立推送傳送](../../push/create-push.md)
>

## 在行銷活動工作流程中建立傳遞{#create-a-delivery-in-a-workflow}

若要在行銷活動工作流程內容中建立電子郵件、簡訊或推播傳送，請遵循下列步驟：

1. 請確保您已新增「**建置對象**」活動。對象是傳遞的主要目標：收到訊息的收件者。在行銷活動工作流程中傳送訊息時，訊息對象不會在管道活動中定義，而是在「**建置對象**」活動中定義。請參閱[本節](build-audience.md)。

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 選取傳遞活動：**[!UICONTROL 電子郵件]**、**[!UICONTROL 簡訊]**、**[!UICONTROL 推播通知 (Android)]** 或&#x200B;**[!UICONTROL 推播通知 (iOS)]**。

1. 選取傳遞&#x200B;**範本**。範本是預先設定的傳遞設定 (特定於管道)。每個管道都會有一個內建範本，並且在預設情況下會預先填寫。[了解更多](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   您可以從管道活動設定左側窗格中選取另一個範本。如果之前選取的對象和管道不相容，則無法選取範本。若要解決此問題，請更新「**建置對象**」活動，以選取具有正確目標對應的對象。進一步瞭解中的目標對應 [Adobe Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

1. 按一下「**建立傳遞**」。以建立獨立傳遞相同的方式定義訊息設定和內容。您還可以排程和模擬內容。[了解更多](../../msg/gs-messages.md)。

1. 導覽回您的工作流程。 選擇是否要繼續您的工作流程 **產生出站轉變** 如果您想在管道活動後新增轉變。

1. 按一下「**開始**」以啟動您的工作流程。

   預設情況下，開始工作流程會觸發訊息準備階段，但不會立即傳送訊息。

1. 開啟傳遞活動，以確認從「**檢閱並傳送**」按鈕進行傳送。

1. 在您的傳遞儀表板中，按一下「**傳送**」。

## 範例{#cross-channel-workflow-sample}

以下是一個具有分段和兩個傳遞的跨管道工作流程範例。此工作流程會以所有居住在巴黎且對咖啡機感興趣的客戶為目標。針對此母體，會傳送電子郵件給普通客戶，並傳送簡訊給 VIP 用戶端。

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

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
