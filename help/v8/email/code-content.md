---
audience: end-user
title: 撰寫您自己電子郵件內容的程式碼
description: 了解如何撰寫您自己電子郵件內容的程式碼
exl-id: a387bff6-3dc8-421c-9efd-043c16694ef0
TQID: 'https://experienceleague.adobe.com/PPrenfLb4utuqvAsrSitbtZzDHcCehzrOMK4R7L2EMw'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 12%
---
# 撰寫您自己電子郵件內容的程式碼 {#code-content}

使用您自己的&#x200B;**[!UICONTROL 編碼模式]**&#x200B;來匯入原始HTML並編碼您的電子郵件內容。

>[!CAUTION]
>
>此方法需要具備HTML知識。

>[!IMPORTANT]
>
>請勿在您的電子郵件內容中使用HTML `<base>`標籤。 基於安全理由，此標籤不受支援，且可能會阻止您的內容在內容編輯器中載入。 請改用連結和外部資源的絕對網址。

1. 在[電子郵件Designer](get-started-email-designer.md)首頁上，選取&#x200B;**[!UICONTROL 自行編碼]**。

   ![在電子郵件Designer首頁中顯示「自行編碼」選項的熒幕擷圖](assets/code-your-own.png){zoomable="yes"}

1. 將您的原始HTML程式碼輸入或貼到主畫布中。

1. 使用左窗格來存取個人化功能。 [了解更多](../personalization/gs-personalization.md)

   ![在左窗格中顯示具有個人化選項的程式碼編輯器的熒幕擷圖](assets/code-editor-personalization.png){zoomable="yes"}

1. 按一下「**[!UICONTROL 模擬內容]**」按鈕，以使用測試設定檔預覽訊息設計和個人化。 [了解更多](../preview-test/preview-test.md)

1. 程式碼完成後，按一下&#x200B;**[!UICONTROL 儲存並關閉]**&#x200B;以返回訊息建立畫面並完成訊息。