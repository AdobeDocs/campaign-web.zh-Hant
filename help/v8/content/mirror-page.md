---
audience: end-user
title: 向鏡像頁面添加連結
description: 了解如何新增和管理鏡像頁面的連結
badge: label="Alpha" type="Infertitive"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# 向鏡像頁面添加連結{#mirror-page}

鏡像頁面是您電子郵件的線上版本。

雖然大部分的電子郵件用戶端都可以順利轉譯影像，但有些預設集可以避免因安全原因顯示影像。 使用者可以瀏覽至電子郵件的鏡像頁面，例如，當他們嘗試在收件匣中檢視時遇到轉譯問題或影像損毀時。 建議您基於協助工具原因提供線上版本，或鼓勵社交分享。

Adobe Campaign產生的鏡像頁面包含所有個人化資料。

![鏡像連結示例](assets/mirror-page-link.png){width="600" align="left"}

## 向鏡像頁面添加連結{#link-to-mirror-page}

插入鏡像頁面的連結是一種好做法。 例如，此連結可以是「在瀏覽器中檢視此電子郵件」或「線上閱讀此內容」。 它通常位於電子郵件的標題或注腳。

在Adobe Campaign中，您可以使用專用 **個人化區塊**. 內建 **鏡像頁面的連結** 個人化區塊會在您的電子郵件內容中插入下列程式碼： `<%@ include view='MirrorPage' %>`.

若要將連結新增至電子郵件中的鏡像頁面：

1. 選取元素並按一下 **[!UICONTROL 插入連結]** 中。

   ![](assets/message-tracking-mirror-page.png)

1. 選取 **[!UICONTROL 插入連結]** 圖示來存取個人化功能表。

   ![](assets/message-tracking-mirror-page_2.png)

1. 從 **[!UICONTROL 內容區塊]** 菜單，選擇 **[!UICONTROL 鏡像頁面URL]** 按一下 **[!UICONTROL 新增]**.

   ![](assets/message-tracking-mirror-page_3.png)

   如需插入自訂內容區塊的詳細資訊，請參閱 [本節](../personalization/personalize.md#personalize-emails).

鏡像頁面會自動建立。

>[!IMPORTANT]
>
>鏡像頁面連結會自動產生，且無法編輯。 它們包含呈現原始電子郵件所需的所有加密個人化資料。 因此，使用具有大值的個人化屬性可能會產生長的鏡像頁面URL，而這會使連結無法在URL長度上限的網頁瀏覽器中運作。

傳送電子郵件後，當收件者按一下鏡像頁面連結時，電子郵件的內容會顯示在其預設的網頁瀏覽器中。

>[!NOTE]
>
>在傳送至測試設定檔的測試電子郵件中，鏡像頁面的連結未作用中。 它只會在最終訊息中啟動。

依預設，鏡像頁面的保留期為60天。 延遲後，鏡像頁面將不再可用。


## 鏡像頁面生成{#mirror-page-generation}

依預設，如果電子郵件內容不為空，且包含鏡像頁面的連結（亦稱為鏡像連結），則Adobe Campaign會自動產生鏡像頁面。

您可以控制電子郵件鏡像頁面的產生模式。 傳遞屬性中提供選項。 [了解更多](../advanced-settings/delivery-settings.md#mirror)
