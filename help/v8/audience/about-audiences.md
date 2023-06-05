---
audience: end-user
title: 開始使用對象
description: 了解如何在 Campaign Web UI 中使用對象
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 53%

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


對象是傳遞的主要目標：接收訊息的收件者。 對象類型取決傳遞範本中定義的目標對應。請參閱本[章節](../msg/delivery-template.md)。

瞭解如何使用Campaign規則產生器並定義篩選條件來選取訊息的對象。 您可以輕鬆使用外部檔案中的資料，或鎖定Adobe Experience Platform對象。


若要定義對象，您可以：

* 選取在使用者端主控台中建立的現有對象。 [了解更多](add-audience.md)
* 使用規則產生器建立新的對象。 [了解更多](segment-builder.md)
* 使用外部檔案中的對象。 [了解更多](file-audience.md)
* 使用 Adobe Experience Platform 對象。[了解更多](aep-audience.md)

此外，您可以定義控制組來避免傳送訊息給對象的其中一部分，以及測量行銷活動的影響。[了解更多](control-group.md)

![](assets/about-audience.png)

