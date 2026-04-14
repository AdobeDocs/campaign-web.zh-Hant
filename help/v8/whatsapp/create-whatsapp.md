---
audience: end-user
title: 建立WhatsApp傳遞
description: 瞭解如何在Adobe Campaign網頁使用者介面中建立WhatsApp傳送
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
source-git-commit: aa1a7c48d1708e73e4d6c6bbe4decd2e5ca69102
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 3%

---


# 建立WhatsApp訊息 {#create-whatsapp}

**Adobe Campaign Web使用者介面**&#x200B;可讓您設計使用Meta核准範本的WhatsApp訊息、為每個設定檔個人化訊息，以及在傳送前測試訊息。


+++ 深入瞭解支援的訊息元素和動作要求

WhatsApp支援下列訊息型別：

| 訊息功能 | 說明 |
|-|-|
| 標頭 | 顯示在訊息本文上方的可選文字。 |
| 文字 | 透過引數支援動態內容。 |
| 頁首影像 | 顯示在訊息本文上方的可選影像。 |
| 內文 | 透過引數支援動態內容。 |
| 頁尾文字 | 透過引數支援動態內容。 |

+++


## 建立WhatsApp傳遞 {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>目前不支援WhatsApp訊息回饋。

在Adobe Campaign網頁使用者介面中，依照下列步驟建立獨立的WhatsApp傳送。

1. 瀏覽至&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 建立傳遞]**。

   ![](assets/whatsapp-create-1.png)

1. 選擇&#x200B;**[!UICONTROL WhatsApp]**&#x200B;並選取傳遞範本。 [進一步瞭解範本](../msg/delivery-template.md)。

   ![](assets/whatsapp-create-2.png)

1. 按一下&#x200B;**[!UICONTROL 建立傳遞]**&#x200B;以進行確認。

1. 按一下&#x200B;**[!UICONTROL 設定]**&#x200B;以取得與範本繫結的進階選項。 [了解更多](../advanced-settings/delivery-settings.md)

   ![](assets/whatsapp-create-3.png)

1. 輸入傳遞的&#x200B;**[!UICONTROL 標籤]**。 若您需要內部名稱、資料夾、傳遞代碼、說明或性質，且與其他管道相同的模式，請使用&#x200B;**[!UICONTROL 其他選項]**。

1. 按一下「**[!UICONTROL 選取對象]**」以鎖定現有對象或建立對象。 [進一步瞭解對象](../audience/about-recipients.md)。

1. 按一下&#x200B;**[!UICONTROL 編輯內容]**&#x200B;以開啟WhatsApp內容編輯器，請參閱[定義您的WhatsApp內容](#whatsapp-content)。

   ![](assets/whatsapp-create-4.png)

1. 您可以啟用&#x200B;**[!UICONTROL 啟用排程]**，以便在特定的日期和時間傳送。 [了解更多資訊](../msg/gs-deliveries.md#gs-schedule)。


## 定義您的WhatsApp內容{#whatsapp-content}

>[!BEGINSHADEBOX]

在Adobe Campaign網頁使用者介面中設計WhatsApp訊息之前，請先在Meta中建立並提交範本。 [了解更多](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

您的WhatsApp範本必須由Meta核准才能使用。 核准通常需要數小時，但最多可能需要24小時。 [了解更多](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. 從Adobe Campaign Web使用者介面的傳遞設定頁面，按一下&#x200B;**[!UICONTROL 編輯內容]**&#x200B;以設定WhatsApp訊息。

1. 選擇行銷作為您的&#x200B;**範本類別**：

   [進一步瞭解範本類別](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

   ![](assets/whatsapp-design-1.png)

1. 從&#x200B;**WhatsApp範本**&#x200B;下拉式清單中，選取您的Meta核准範本。

   [進一步瞭解如何建立WhatsApp範本](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

   ![](assets/whatsapp-design-2.png)

1. 如果您的Meta核准範本包含影像，請提供&#x200B;**[!UICONTROL 影像URL]**。

   ![](assets/whatsapp-design-3.png)

1. 在&#x200B;**Personalization預留位置**&#x200B;欄位中，使用個人化編輯器將設定檔欄位和運算式對應至範本引數。 [了解更多資訊](../personalization/personalize.md)。

   ![](assets/whatsapp-design-4.png)

訊息就緒時：

* **獨立或行銷活動傳遞**：在傳遞控制面板上使用&#x200B;**[!UICONTROL 檢閱與傳送]**&#x200B;和&#x200B;**[!UICONTROL 傳送]**。

* **工作流程**：在執行使其可用時，從工作流程活動開啟傳遞，然後以相同方式使用傳遞儀表板。 [了解更多](../workflows/start-monitor-workflows.md)

然後，您可以追蹤傳遞&#x200B;**[!UICONTROL 報告]**&#x200B;進入點和[傳遞報告](../reporting/delivery-reports.md)的結果。
