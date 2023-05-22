---
audience: end-user
title: 使用工作流程管道活動
description: 了解如何將管道活動用於 Adobe Campaign Web 工作流程
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 26%

---

# 管道活動 {#channel}

Adobe CampaignWeb使您能夠跨多個渠道（如電子郵件、簡訊或推送）自動執行營銷活動。 使用Adobe Campaign工作流，您可以將渠道活動組合到畫布中，以建立跨渠道工作流，這些工作流可以根據客戶行為觸發操作。

例如，您可以建立歡迎電子郵件活動，該活動包括跨不同渠道的一系列消息，如電子郵件、簡訊和推送。 您還可以在客戶完成購買後發送電子郵件或通過簡訊向客戶發送個性化生日消息。

通過使用渠道活動，您可以建立全面、個性化的活動，讓客戶跨多個觸點進行接觸並進行驅動器轉換。

頻道活動可從螢幕左側的「頻道」部分的調色板獲得。

## 電子郵件 {#email}

說明，您可以執行哪個使用案例 (您可以在活動之前或之後連結的其他常見活動)

如何新增和設定活動

工作流程中已設定之活動的範例


「電子郵件傳遞」活動允許您配置在工作流中發送電子郵件。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

電子郵件收件人是通過「受眾目標」活動在同一工作流中活動的上游定義的。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->