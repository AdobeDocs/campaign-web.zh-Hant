---
audience: end-user
title: 使用工作流程活動
description: 瞭解如何工作流程活動
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 4c0157c0457d1d6fa3194463adef8572017af8f0
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 5%

---


# 關於工作流程活動 {#workflow-activities}

工作流程活動分為三個類別。 根據內容的不同，可用的活動可能會有所不同。

以下各節將詳細說明所有活動：

* [目標定位活動](#targeting)
* [管道活動](#channel)
* [流程控制活動](#flow-control)

## 目標定位活動 {#targeting}

這些活動專門用於定位、操控和豐富人口資料。 它們可讓您定義對象，並使用交集、聯合或排除作業來分割或結合這些對象，藉此建立一或多個目標。

* 此 [建立對象](build-audience.md) 活動可讓您定義目標母體。 您可以選取現有對象，或使用規則產生器來定義自己的查詢。
* 此 [合併](combine.md) 活動可讓您對入站母體執行分段。 您可以使用聯集、交集或排除。
* 此 [擴充](enrichment.md) 活動可讓您定義要在工作流程中處理的其他資料。 透過此活動，您可以運用入站轉變，並設定活動以使用其他資料完成輸出轉變。

## 管道活動 {#channel}

Adobe Campaign Web可讓您跨多個管道（例如電子郵件、簡訊或推播）自動執行行銷活動。 透過Adobe Campaign工作流程，您可以將管道活動結合到畫布中，以建立可根據客戶行為觸發動作的跨管道工作流程。

例如，您可以建立歡迎電子郵件行銷活動，其中包括跨不同頻道的一系列訊息，例如電子郵件、簡訊和推播。 客戶完成購買後，您也可以傳送後續追蹤電子郵件，或透過簡訊傳送個人化生日訊息給客戶。

透過使用管道活動，您可以建立全面、個人化的行銷活動，在多個接觸點吸引客戶並促進轉換。

* [電子郵件](email.md)
* [推播](push.md)
* [SMS](sms.md)

## 流程控制活動 {#flow-control}

以下活動專用於組織和執行工作流程。 他們的主要工作是協調其他活動：

* 此 [合併連結](and-join.md) 活動可讓您同步工作流程的多個執行分支。
* 此 [結束](end.md) 活動為選用。 您可以使用
* 此 [分支](fork.md) 活動可讓您建立出站轉變，以同時開始多個活動。
* 此 [等待](wait.md) 活動會暫時暫停執行工作流程的一部分。

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

