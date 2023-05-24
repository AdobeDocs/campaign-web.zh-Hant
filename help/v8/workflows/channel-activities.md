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

Adobe Campaign Web可讓您跨多個管道（例如電子郵件、簡訊或推播）自動執行行銷活動。 透過Adobe Campaign工作流程，您可以將管道活動結合到畫布中，以建立可根據客戶行為觸發動作的跨管道工作流程。

例如，您可以建立歡迎電子郵件行銷活動，其中包括跨不同頻道的一系列訊息，例如電子郵件、簡訊和推播。 客戶完成購買後，您也可以傳送後續追蹤電子郵件，或透過簡訊傳送個人化生日訊息給客戶。

透過使用管道活動，您可以建立全面、個人化的行銷活動，在多個接觸點吸引客戶並促進轉換。

頻道活動可從畫面左側的「頻道」區段的浮動視窗中使用。

## 電子郵件 {#email}

說明，您可以執行哪個使用案例 (您可以在活動之前或之後連結的其他常見活動)

如何新增和設定活動

工作流程中已設定之活動的範例


電子郵件傳送活動可讓您在工作流程中設定傳送電子郵件。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

電子郵件收件者是透過對象鎖定目標活動，在相同工作流程中定義活動上游的活動。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->