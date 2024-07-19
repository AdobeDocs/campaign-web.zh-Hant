---
audience: end-user
title: 排程傳送作業
description: 瞭解如何排程傳遞
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# 排程傳送作業 {#schedule-sending}

您可以排程傳遞的傳送。 此步驟將取決於其為獨立（一次性）傳遞，或您是否正於行銷活動工作流程的內容中工作。

## 獨立傳送

對於獨立傳送，您可以直接排程傳送的日期和時間。
如需各種傳送型別的詳細資訊，請參閱以下範例：電子郵件、簡訊、推播通知。

### 電子郵件 {#schedule-email-standalone}

若要排程電子郵件傳送的傳送，請遵循下列步驟：

1. 在傳遞屬性的&#x200B;**[!UICONTROL 排程]**&#x200B;區段中，啟動&#x200B;**[!UICONTROL 啟用排程]**&#x200B;切換按鈕

1. 設定所要的傳送日期和時間，然後按一下&#x200B;**[!UICONTROL 檢閱並傳送]**&#x200B;按鈕。

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>預設會選取「**[!UICONTROL 啟用傳送前確認]**」選項。此選項要求您在排程的日期和時間傳遞之前確認傳送。若您需要在排程的日期與時間自動&#x200B;**傳送傳遞**，您必須停用此選項。
>

1. 檢查排程是否正確，然後按一下&#x200B;**[!UICONTROL 準備]**&#x200B;按鈕。

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. 準備完成後，訊息即可傳送。 顯示傳遞的關鍵量度：目標人口總數、要傳遞的訊息數、排除的收件者數。 按一下&#x200B;**[!UICONTROL 依排程傳送]**&#x200B;按鈕，確認您允許在排程的日期和時間傳送傳遞至主要目標。

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### 簡訊

若要將簡訊傳送排程在特定日期和時間，步驟與電子郵件傳送相同，[請參閱上文](#schedule-email-standalone)。

![](assets/schedule-sms-standalone.png){zoomable="yes"}

您也可以檢查是否已將排程納入考量：

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### 推播通知

若要將獨立推播傳送排程至特定日期和時間，步驟與電子郵件傳送相同，[請參閱上文](#schedule-email-standalone)。

![](assets/schedule-push-standalone.png){zoomable="yes"}

您也可以檢查是否已將排程納入考量：

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### 行銷活動中的獨立傳送

您無需使用工作流程，即可在行銷活動中建立獨立傳送。 您可以設定此傳送的日期和時間排程，如上所述。
行銷活動可能有其排程，包含開始日期和結束日期。 此排程不會影響您的傳送排程。

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## 在行銷活動工作流程中排程傳遞

在行銷活動工作流程的內容中，**最佳實務**&#x200B;是使用&#x200B;**[!UICONTROL 排程器]**&#x200B;活動來套用將啟動工作流程的日期和時間，包括傳送傳遞。 [進一步瞭解排程器](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


您必須在&#x200B;**[!UICONTROL 排程器]**&#x200B;活動中設定日期和時間。

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>當您使用&#x200B;**[!UICONTROL 排程器]**&#x200B;活動在工作流程中排程傳送您的傳遞時，**請勿啟用** **[!UICONTROL 傳遞]**&#x200B;活動設定中的&#x200B;**[!UICONTROL 啟用排程]**&#x200B;切換。 系統會自動傳送您的傳遞。
>

若您在&#x200B;**[!UICONTROL 傳遞]**&#x200B;活動設定中啟用&#x200B;**[!UICONTROL 啟用排程]**&#x200B;切換功能，並設定日期和時間，則傳遞將在此日期和時間等候傳送。 這表示如果工作流程啟動日期和傳送日期之間有延遲，則對象可能不是最新狀態。
