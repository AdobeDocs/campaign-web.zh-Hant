---
audience: end-user
title: 使用持續傳遞工作流程活動
description: 瞭解如何使用持續傳遞工作流程活動
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
TQID: https://experienceleague.adobe.com/uWGhvUmHdS0ixFI4d-uEPgpxSnZoOwNRMbn8aZfqA98
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 24%

---

# 持續傳遞 {#continuous-delivery}

**持續傳遞**&#x200B;活動可讓您新增收件者到現有的傳遞。 此傳遞類型不需要每次都建立新的傳遞，對於少量的警示或依需求傳送的通知而言，能大幅提升效率。

一個持續傳遞建立一個傳遞實例。 所有傳遞記錄 (broadLog) 和追蹤記錄都參考這個傳遞，藉此簡化監控和報告。

## 設定持續傳遞活動 {#configure}

1. 將&#x200B;**持續傳遞**&#x200B;活動新增至工作流程畫布。

   ![顯示持續傳遞活動的熒幕擷圖](../assets/continuous-delivery.png){zoomable="yes"}

1. 輸入活動的自訂&#x200B;**[!UICONTROL 標籤]** （選擇性）。 依預設，其標籤為「持續傳遞」。

1. 在&#x200B;**[!UICONTROL 範本]**&#x200B;欄位旁邊，按一下搜尋圖示以選取傳遞範本。 僅範本（非標準傳送）可供選取。 範本會定義傳遞管道、內容和設定。

1. 在&#x200B;**[!UICONTROL 目標定位選項]**&#x200B;中，選擇目標母體的定義方式：

   * **[!UICONTROL 由入站事件指定]**：目標來自入站轉變（來自上游活動，例如建置對象或增量查詢）。 這是最常見的選項。

   * **[!UICONTROL 已在傳遞範本中指定]**：目標已在範本本身中定義。

   * **[!UICONTROL 在輸入事件中指定的檔案]**：目標是由透過工作流程傳遞的檔案所提供。

持續傳遞活動會自動產生出站轉變，以繼續您的工作流程。

## 相關主題 {#related}

* [關於工作流程活動](about-activities.md)
* [自動化傳遞](automated-delivery.md)
* [電子郵件、簡訊、推播、直接郵件活動](channels.md)
* [傳遞範本](../../msg/delivery-template.md)
