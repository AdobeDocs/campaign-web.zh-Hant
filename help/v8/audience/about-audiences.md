---
audience: end-user
title: 開始使用對象
description: 了解如何在 Campaign Web UI 中使用對象
badge: label="Alpha"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '215'
ht-degree: 100%

---


# 開始使用對象 {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


對象是傳遞的主要目標：收到訊息的收件者。對象類型會依據傳遞範本中定義的目標對應而不同。若要了解什麼是傳遞範本，請參閱[本章節](../msg/delivery-template.md)。

若要定義對象族群，您可以：

* 選取現有對象，在用戶端主控台中建立成清單。[了解更多](add-audience.md)
* 選取 Adobe Experience Platform 對象。[了解更多](aep-audience.md)
* 定義篩選條件並將其合併，以使用規則產生器建置新的對象。[了解更多](segment-builder.md)
* 使用來自外部檔案的對象：此選項僅適用於獨立的電子郵件傳遞，不能用於行銷活動傳遞。[了解更多](file-audience.md)

在行銷活動工作流程中傳送訊息時，會在特定的&#x200B;**讀取對象**&#x200B;工作流程活動中定義對象。在此特定情況下，您無法從檔案載入對象以進行電子郵件傳遞，並且該對象的定義僅適用於此專用活動。若要了解如何在行銷活動工作流程中定義傳遞的對象，請參閱[本章節](../workflows/orchestrate-activities.md)。

此外，您可以定義控制組來避免傳送訊息給對象的其中一部分，以及測量行銷活動的影響。[了解更多](control-group.md)

![](assets/about-audience.png)

