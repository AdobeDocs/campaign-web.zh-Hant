---
audience: end-user
title: 新增鏡像頁面連結
description: 了解如何新增和管理鏡像頁面連結
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 16%

---

# 鏡像頁面 {#mirror-page}

映象頁面是電子郵件的線上版本。 在電子郵件行銷中，將連結新增至映象頁面是很好的做法。 例如，使用者在收件匣中檢視電子郵件時遇到轉譯問題或影像損毀時，可以存取該電子郵件的映象頁面。 也建議基於協助工具原因或鼓勵社交分享，提供線上版本。

Adobe Campaign產生的映象頁面包含所有個人化資料。

![電子郵件中的映象連結範例](assets/mirror-page-link.png){width="600" align="left"}

## 新增鏡像頁面連結 {#link-to-mirror-page}

在Adobe Campaign中，使用專用的&#x200B;**個人化區塊**，在電子郵件內容中插入映象頁面的連結。 內建的&#x200B;**鏡像頁面連結**&#x200B;個人化區塊會將以下程式碼插入電子郵件內容中：`<%@ include view='MirrorPage' %>`。

若要在電子郵件中新增映象頁面的連結，請執行下列步驟：

1. 選取元素（文字或影像），然後按一下內容工具列中的[插入連結]。**&#x200B;**

   ![顯示[插入連結]選項的內容工具列](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. 選取「**[!UICONTROL 新增個人化]**」圖示，以存取個人化選單。

   Adobe Campaign中的![Personalization功能表](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. 從&#x200B;**[!UICONTROL 片段]**&#x200B;功能表選取&#x200B;**[!UICONTROL 映象頁面URL]**，然後按一下&#x200B;**[!UICONTROL 新增]**。 [瞭解如何使用運算式片段](../content/use-expression-fragments.md)

   ![片段功能表中的映象頁面URL選項](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

鏡像頁面會自動建立。

傳送電子郵件時，按一下映象頁面連結的收件者會看到其預設網頁瀏覽器中顯示的電子郵件內容。

依預設，映象頁面的保留期間為&#x200B;**60天**。 在此期間後，將無法再使用映象頁面。

>[!CAUTION]
>
>* 映象頁面連結會自動產生，且無法編輯。 這些檔案包含轉譯原始電子郵件所需的所有加密個人化資料。 使用具有大型值的個人化屬性可能會產生過長的映象頁面URL，使得連結無法在URL長度上限的網頁瀏覽器中運作。
>
>* 在傳送給測試設定檔的校樣中，指向映象頁面的連結未啟用。 它只會在最終訊息中處於活動狀態。

## 鏡像頁面產生 {#mirror-page-generation}

根據預設，如果電子郵件內容不是空的，且包含映象頁面的連結（也稱為映象連結），Adobe Campaign會自動產生映象頁面。

透過傳遞屬性中可用的選項，控制電子郵件映象頁面的產生模式。 [了解更多](../advanced-settings/delivery-settings.md#mirror)