---
audience: end-user
title: 開始使用對象
description: 了解如何在 Campaign Web UI 中使用對象
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: bbebd9dc462a189618cbf6e71467bb0935e1317a
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 31%

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


對象是傳遞的主要目標：接收訊息的收件者。 對象類型取決傳遞範本中定義的目標對應。瞭解什麼是傳遞範本 [在本節中](../msg/delivery-template.md).

若要定義對象母體，您可以：

* 選取在使用者端主控台中建立為清單的現有對象。 [了解更多](add-audience.md)
* 選取Adobe Experience Platform對象。 [了解更多](aep-audience.md)
* 定義並結合篩選條件，以使用規則產生器建立新對象。 [了解更多](segment-builder.md)
* 使用外部檔案中的對象：此選項僅適用於獨立電子郵件傳送，無法用於行銷活動傳送。 [了解更多](file-audience.md)

在行銷活動工作流程內容中傳送訊息時，對象會定義於特定的 **讀取對象** 工作流程活動。 在此內容中，您無法從檔案載入對象以進行電子郵件傳送，而且對象僅定義在此專用活動中。 瞭解如何在行銷活動工作流程中定義傳送的對象 [在本節中](../workflows/orchestrate-activities.md).

此外，您可以定義控制組來避免傳送訊息給對象的其中一部分，以及測量行銷活動的影響。[了解更多](control-group.md)

![](assets/about-audience.png)

