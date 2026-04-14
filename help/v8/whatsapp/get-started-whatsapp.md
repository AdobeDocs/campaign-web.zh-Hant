---
audience: end-user
title: 開始使用WhatsApp訊息
description: 瞭解如何使用Adobe Campaign網頁使用者介面建立和傳送WhatsApp訊息
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---

# 開始使用WhatsApp訊息 {#get-started-whatsapp}

您可以使用Meta的&#x200B;**Cloud API**，從[Adobe Campaign Web使用者介面](https://developers.facebook.com/docs/whatsapp/cloud-api/)傳送WhatsApp訊息。 將WhatsApp用於獨立傳送、行銷活動工作流程，或行銷活動內，連同您的其他管道。

* **[!UICONTROL 傳遞]**：在Adobe Campaign網頁使用者介面中，從左側邊欄的&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表建立獨立的WhatsApp傳遞，類似SMS或推播。 [了解更多資訊](create-whatsapp.md)。

* **[!UICONTROL 行銷活動]**：在Adobe Campaign網路使用者介面中，從&#x200B;**[!UICONTROL 傳送]**&#x200B;索引標籤開啟行銷活動並新增WhatsApp傳送，或協調傳送並附加至行銷活動的工作流程。 [了解更多資訊](../campaigns/create-campaigns.md)。

* **[!UICONTROL 工作流程]**：在Adobe Campaign網頁使用者介面的工作流程畫布中，新增&#x200B;**[!UICONTROL WhatsApp]**&#x200B;頻道活動、選擇傳遞範本，然後在傳遞控制面板中定義內容和設定。 在[本節](../workflows/activities/channels.md)中進一步瞭解管道活動。

## 先決條件 {#prereq}

整合WhatsApp需要下列專案：

* Meta Business Manager帳戶
* [具有已驗證寄件者名稱與電話號碼的WhatsApp商業帳戶](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [具有適當許可權的使用者授權權杖](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [已核准的Meta範本](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

在繼續之前，您還需要確認下列事項：

* [WhatsApp內容規則](https://www.whatsapp.com/legal/messaging-guidelines)
* [符合Meta原則](https://www.whatsapp.com/legal)
* [24小時交談限制](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


