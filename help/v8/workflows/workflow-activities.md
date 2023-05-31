---
audience: end-user
title: 使用工作流程活動
description: 瞭解如何工作流程活動
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c134f930b253a8d4463f438176fc54e09ea21a48
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 74%

---


# 工作流程活動 {#workflow-activities}

## 目標定位活動 {#targeting}

內容待定

<!--à reformuler-->這些活動可讓您使用交集、聯合或執行運算來定義組合和分割或結合這些組合，藉此建置一個或多個目標。

### 建置對象 {#build-audience}

### 組合 {#combine}

### 擴充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="擴充活動"
>abstract="擴充活動可讓您使用資料庫中的其他資訊來增強目標資料。它通常在目標定位活動之後用於工作流程。<br/>將擴充資料新增到工作流程後，它可以用於在擴充活動之後新增的活動中，根據客戶的行為、偏好和需求將客戶分成不同群組，或是用於建立最有可能讓目標對象產生共鳴的個人化行銷訊息和行銷活動。"

擴充活動可讓您使用資料庫中的其他資訊來增強目標資料。它通常在目標定位活動之後用於工作流程。

擴充資料可以：

* **來自相同工作表**，作為您工作流程中的目標：

   *以一組客戶為目標，並新增「生日」欄位到目前工作表*

* **來自另一個工作表**：

   *以一組客戶為目標，並新增來自「購買」表格的「數量」和「產品類型」欄位*。

將擴充資料新增到工作流程後，它可以用於在擴充活動之後新增的活動中，根據客戶的行為、偏好和需求將客戶分成不同群組，或是用於建立最有可能讓目標對象產生共鳴的個人化行銷訊息和行銷活動。

例如，您可以將與客戶購買行為相關資訊新增到工作流程的工作表中，並使用此資料根據客戶上次購買行為或消費金額來個人化電子郵件。

若要將擴充活動新增到您的工作流程，請依照以下步驟操作：

1. 新增活動
1. 選取屬性做為擴充資料

   顯示進階欄位選項
i 按鈕

   注意：來自目標維度的屬性

1. 選取資料收集方式
1. 要擷取的記錄數 (如果要擷取多個記錄的集合)
1. 套用篩選和建置規則

   選取現有篩選器
儲存篩選器以重複使用
以視覺化方式或在程式碼檢視中檢視篩選結果

1. 使用屬性排序記錄

在行銷活動中利用擴充資料

可以在哪裡使用擴充資料：個人化電子郵件或其他使用案例？


## 管道活動 {#channel}

Adobe Campaign Web可讓您跨多個管道（例如電子郵件、簡訊或推播）自動執行行銷活動。 透過Adobe Campaign工作流程，您可以將管道活動結合到畫布中，以建立可根據客戶行為觸發動作的跨管道工作流程。

例如，您可以建立歡迎電子郵件行銷活動，其中包括跨不同頻道的一系列訊息，例如電子郵件、簡訊和推播。 客戶完成購買後，您也可以傳送後續追蹤電子郵件，或透過簡訊傳送個人化生日訊息給客戶。

透過使用管道活動，您可以建立全面、個人化的行銷活動，在多個接觸點吸引客戶並促進轉換。

頻道活動可從畫面左側的「頻道」區段的浮動視窗中使用。

### 電子郵件 {#email}

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


### SMS {#sms}

### 推播通知 (Android) {#push-android}

### 推播通知 (iOS) {#push-ios}

## 流程控制活動 {#flow-control}

內容待定

<!--à reformuler-->這些活動可讓您使用交集、聯合或執行運算來定義組合和分割或結合這些組合，藉此建置一個或多個目標。

流程控制活動用於協調工作流程活動。

### 分支 {#fork}

### AND-join {#join}


### 等待 {#wait}

### 結束 {#end}

## 資料管理活動 {#data-management}

概觀：它們的用途
它們適用的使用案例

列出可用的活動 + 簡短說明 + 參考章節

