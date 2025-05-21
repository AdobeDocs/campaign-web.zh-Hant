---
audience: end-user
title: 關於隔離
description: 瞭解隔離地址的管理
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# 隔離管理 {#quarantines}

Adobe Campaign會管理電子郵件、推播和簡訊通道的隔離地址。

隔離僅適用於&#x200B;**電子郵件地址**、**電話號碼**&#x200B;或&#x200B;**裝置權杖**，但不適用於設定檔本身。 例如，已隔離電子郵件地址的設定檔可更新為新地址。 然後，設定檔可能會再次被傳遞動作設為目標。 同樣地，如果兩個設定檔共用相同的電話號碼，則兩個設定檔在隔離該號碼時都會受到影響。

>[!CAUTION]
>
>Adobe Campaign中的隔離區會區分大小寫。

## 什麼是隔離 {#quarantines-what}

隔離是用於&#x200B;**管理傳遞中的無效地址**&#x200B;的方法。

如果傳送的無效位址比率很高，則可能會被視為垃圾訊息。 透過隔離管理這些位址，有助於防止網際網路提供者將其列入封鎖清單。 這對於維護您的聲譽很重要。

在Adobe Campaign中隔離地址時，設定檔會在傳送分析期間自動從目標中排除。

隔離功能可將錯誤的電話號碼排除在遞送服務之外，藉此降低SMS傳送成本。

在[Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}中進一步瞭解隔離。

## 為何將地址傳送至隔離區 {#quarantines-why}

許多原因都可能導致地址被隔離：

* 針對簡訊，錯誤的電話號碼
* 針對簡訊，當設定檔回覆具有關鍵字（例如「STOP」）的簡訊時
* 針對電子郵件，在您的郵件回報為垃圾郵件時。 郵件會自動重新導向至Adobe管理的技術信箱。 之後，系統會自動將使用者的電子郵件地址傳送到狀態為「已加入封鎖清單」的隔離區。
* 舉例來說，信箱已滿、地址不存在或電子郵件伺服器無法使用時，可以隔離電子郵件地址。

在[Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}中進一步瞭解傳遞失敗。

## 在何處尋找隔離地址 {#quarantines-where}

您可以在&#x200B;**[!UICONTROL 總管]** > **[!UICONTROL 管理]** > **[!UICONTROL 行銷活動管理]** > **[!UICONTROL 無法傳遞的專案管理]** > **[!UICONTROL 無法傳遞的專案和地址]**&#x200B;中檢視執行個體中的所有隔離地址。 本節列出電子郵件、簡訊和推播通知通道的隔離元素。

![Adobe Campaign介面中的隔離位置](assets/quarantine_location.png){zoomable="yes"}

您也可以存取執行個體中隔離的相關報告：

![Adobe Campaign介面中的隔離報告](assets/quarantine_reports.png){zoomable="yes"}

對於每次傳遞，您可以檢查傳遞摘要報告。 它會顯示傳送目標中隔離的地址數量：

![顯示隔離地址的傳遞摘要報告](assets/quarantine_delivery.png){zoomable="yes"}

您可以探索更多選項，以在Adobe Campaign主控台中管理隔離地址。 [了解更多](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)。