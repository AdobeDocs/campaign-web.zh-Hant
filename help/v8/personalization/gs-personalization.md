---
title: 開始使用動態內容
description: 瞭解如何使用個人化、條件式內容和內建內容區塊，讓您的內容成為動態內容。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 12%

---


# 開始使用動態內容

向客戶傳遞相關內容是確保您吸引各種客戶並發揮其興趣以便讀取行銷內容的關鍵。

為了充分運用每個行銷活動，Adobe Campaign可讓您利用所收集關於客戶的資訊，提供與客戶在不同層級對話的自訂動態內容，藉此建立不同群組和個人的自訂體驗。

* **個人化您的訊息** 每個特定收件者可透過運用設定檔資料，例如其名字、興趣、居住地、購買內容等。

  您可以從與收件者、訊息或傳遞相關的個人化編輯器中選取資料庫中可用的任何欄位。 這些個人化屬性可以插入訊息的主旨行或內文中。以下語法將收件者城市插入您的內容：&lt;%= recipient.location.city %>。

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **建立條件式內容** 將您的傳遞調整至每位收件者，並根據您擁有的客戶相關資訊僅顯示與指定客戶相關的內容。 這可讓您根據條件顯示特定的文字區塊和/或影像。 例如，根據收件者對特定服務的訂閱，調整電子郵件橫幅。

  ![](assets/condition-sample.png){width="800" align="center"}

* **使用個人化區塊** 以節省時間，並將可輕鬆重複使用的個人化內容用於訊息。 Campaign 隨附一組個人化區塊，其中包含您可以插入到傳遞中的特定轉譯。例如，您可以新增標誌、問候語訊息，或電子郵件訊息映象頁面的連結。 可從個人化編輯器中的專用專案取得內容區塊。

  ![](assets/content-blocks.png){width="800" align="center"}

## 存取運算式編輯器 {#access}

Adobe Campaign V8 Web提供運算式編輯器，您可在其中選取、排列、自訂及驗證所有資料，以建立內容的自訂體驗。 運算式編輯器適用於所有管道，在每個欄位中具有 **[!UICONTROL 開啟個人化對話方塊]** 圖示，例如主旨行欄位，或電子郵件連結和文字/按鈕內容元件。

以下是如何根據您要建立動態的內容來存取運算式編輯器的部分範例：

* *從「寄件者名稱」欄位存取運算式編輯器*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *從電子郵件文字元件存取運算式編輯器*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *從電子郵件中的連結存取運算式編輯器*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>除了運算式編輯器之外，在設計電子郵件時，您還可以運用專用的條件式內容產生器。 [瞭解如何在電子郵件中建立條件式內容](conditions.md)

## 讓我們深入探討

現在您已瞭解如何讓內容充滿活力，是時候深入探討這些檔案區段來開始使用功能了。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="將內容個人化" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>新增個人化</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="銷售機會" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>新增條件式內容</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="不常使用" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>新增內建內容區塊</strong></a>
</div>
<p></td>
</tr></table>
