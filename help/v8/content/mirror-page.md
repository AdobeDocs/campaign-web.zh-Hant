---
audience: end-user
title: 新增鏡像頁面連結
description: 了解如何新增和管理鏡像頁面連結
badge: label="Alpha" type="Positive"
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 05d87fc9ff8f5e2038eba4cc9438e058566e04c8
workflow-type: ht
source-wordcount: '443'
ht-degree: 100%

---

# 新增鏡像頁面連結{#mirror-page}

鏡像頁面是您電子郵件的線上版本。

雖然大部分電子郵件用戶端可以正確轉譯影像，但是某些預設集可以基於安全原因避免顯示影像。使用者可以瀏覽到電子郵件的鏡像頁面，例如他們在嘗試在收件匣中檢視郵件時遇到轉譯問題或影像毀損。我們建議基於存取性原因或鼓勵社交共享，提供線上版本。

Adobe Campaign 產生的鏡像頁面包含所有個人化資料。

![鏡像連結範例](assets/mirror-page-link.png){width="600" align="left"}

## 新增鏡像頁面連結{#link-to-mirror-page}

插入鏡像頁面連結是很好的做法。例如，此連結可以是「在瀏覽器中檢視此電子郵件」或「線上閱讀」。它通常位於電子郵件的頁首或頁尾。

在 Adobe Campaign 中，您可以使用專屬 **個人化區塊**，將鏡像頁面連結插入電子郵件中。內建的&#x200B;**鏡像頁面連結**&#x200B;個人化區塊會將以下程式碼插入電子郵件內容中：`<%@ include view='MirrorPage' %>`。

若要將鏡像頁面連結新增到您的電子郵件：

1. 選取元素，然後從內容關聯式工具列中按一下「**[!UICONTROL 插入連結]**」。

   ![](assets/message-tracking-mirror-page.png)

1. 選取「**[!UICONTROL 新增個人化]**」圖示，以存取個人化選單。

   ![](assets/message-tracking-mirror-page_2.png)

1. 從「**[!UICONTROL 內容區塊]**」選單，選取「**[!UICONTROL 鏡像頁面 URL]**」，然後按一下「**[!UICONTROL 新增]**」。

   ![](assets/message-tracking-mirror-page_3.png)

   有關自訂容區塊插入的詳細資訊，請參閱[本章節](../personalization/personalize.md#personalize-emails)。

鏡像頁面會自動建立。

>[!IMPORTANT]
>
>鏡像頁面連結是自動產生的，無法編輯。它們包含轉譯原始電子郵件所需的所有加密的個人化資料。因此，使用具有較大值的個人化屬性可能會產生冗長的鏡像頁面 URL，如果網頁瀏覽器具有最大 URL 長度，將導致連結無法在該網頁瀏覽器中作用。

電子郵件傳送後，當收件者按一下鏡像頁面連結時，電子郵件的內容將顯示在他們的預設網頁瀏覽器中。

>[!NOTE]
>
>在傳送到測試設定檔的測試電子郵件中，鏡像頁面連結未啟用。它僅在最終訊息中啟用。

依預設，鏡像頁面的保留期為 60 天。該段時間之後，鏡像頁面無法繼續使用。


## 鏡像頁面產生{#mirror-page-generation}

依預設，如果電子郵件內容不是空的且包含鏡像頁面連結 (也稱為鏡像連結)，Adobe Campaign 會自動產生鏡像頁面。

您可以控制電子郵件鏡像頁面的產生模式。傳遞屬性中有提供相關選項。[了解更多](../advanced-settings/delivery-settings.md#mirror)
