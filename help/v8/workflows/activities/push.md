---
audience: end-user
title: 使用推播通知工作流程活動
description: 瞭解如何使用推播通知工作流程活動
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 5%

---


# 推播通知 {#push-activity}

此 **推播通知** 傳遞活動可讓您設定在工作流程中傳送推播通知。

>[!BEGINTABS]

>[!TAB 推播通知 (Android)]

1. 建立和設定新工作流程後，新增「建立對象」活動以選取現有對象，或使用規則產生器定義您自己的查詢。

1. 將推播通知(Android)通道活動新增至您的工作流程。

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. 選取您的活動。 從傳遞功能表中，選取您要用於此傳遞的範本。 了解範本的詳細資訊

1. 按一下「建立傳送」以設定推播通知傳送。 如需推播通知(Android)傳送的詳細資訊，請參閱本頁面。

1. 一旦您的傳遞準備好傳送，請導覽回您的工作流程，然後按一下「開始」以啟動您的工作流程。

1. 依預設，啟動傳遞工作流程會觸發訊息準備階段，而不會立即傳送訊息。

   從推播通知(Android)頻道活動的進階功能表按一下檢閱和傳送，以確認傳送。

1. 在推播通知傳送控制面板中，按一下傳送。

>[!TAB 推播通知 (iOS)]

1. 建立和設定新工作流程後，新增「建立對象」活動以選取現有對象，或使用規則產生器定義您自己的查詢。

1. 新增推播通知(iOS)通道活動至您的工作流程。

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. 選取您的活動。 從傳遞功能表中，選取您要用於此傳遞的範本。 了解範本的詳細資訊

1. 按一下「建立傳送」以設定推播通知傳送。 如需推播通知(iOS)傳送的詳細資訊，請參閱本頁面。

1. 一旦您的傳遞準備好傳送，請導覽回您的工作流程，然後按一下「開始」以啟動您的工作流程。

1. 依預設，啟動傳遞工作流程會觸發訊息準備階段，而不會立即傳送訊息。

   從推播通知(iOS)頻道活動的進階功能表按一下檢閱和傳送，以確認傳送。

1. 在推播通知傳送控制面板中，按一下傳送。

>[!ENDTABS]