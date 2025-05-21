---
solution: Campaign, Campaign v8 Web User Interface
title: 登陸頁面使用案例
description: 探索Campaign網頁使用者介面中登入頁面最常見的使用案例
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: 登陸、登陸頁面、使用案例
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 9%

---

# 如何使用登陸頁面 {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="請謹慎複製 URL"
>abstract="若要全面測試或善用您的登陸頁面，您不得將此連結直接複製並貼上到網頁瀏覽器或您的傳遞內容中。請改用&#x200B;**模擬內容**&#x200B;功能對其進行測試，並按照文件中所述的步驟正確使用您的登陸頁面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="請謹慎複製 URL"
>abstract="建立登陸頁面時，四個現成的範本可讓您實作不同的使用案例：新增或更新設定檔至行銷活動資料庫、為客戶訂閱服務、取消訂閱服務，或選擇將使用者登出。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?#create-landing-page" text="設定登陸頁面"

若要正確使用登入頁面，請使用專用選項，將其參照為訊息中的連結。 您無法將已發佈傳遞控制面板中顯示的連結直接複製並貼到您的傳遞或網頁中。 請改用&#x200B;**模擬內容**&#x200B;功能來測試。

在[!DNL Adobe Campaign Web]介面中，有四個現成的範本可讓您實作不同的使用案例。 不過，主要步驟保持不變，詳見下文。

1. [建立登入頁面](create-lp.md#create-landing-page)，並根據您的使用案例選取您選擇的範本。

1. 定義登入頁面屬性和設定。

   ![顯示登入頁面屬性和設定介面的熒幕擷圖。](assets/lp-uc-properties.png){zoomable="yes"}

1. 根據您的案例，選取&#x200B;**[!UICONTROL 贏取]**、**[!UICONTROL 訂閱]**、**[!UICONTROL 取消訂閱]**&#x200B;或&#x200B;**[!UICONTROL 封鎖清單]**&#x200B;頁面。

1. 頁面內容隨即顯示。 選取與登入頁面表單相對應的部分。

   ![顯示登入頁面表單介面的熒幕擷圖。](assets/lp-uc-form.png){zoomable="yes"}

1. 根據選取的範本編輯您的內容：

   * [贏取](#lp-acquisition)
   * [訂閱](#lp-subscription)
   * [取消訂閱](#lp-unsubscription)
   * [封鎖清單](#lp-denylist)

1. 視需要修改其餘內容、儲存變更，然後關閉。

1. 視需要編輯&#x200B;**[!UICONTROL Confirmation]**&#x200B;頁面，以及&#x200B;**[!UICONTROL 錯誤]**&#x200B;和&#x200B;**[!UICONTROL 到期]**&#x200B;頁面。 收件者提交表單後，**[!UICONTROL Confirmation]**&#x200B;頁面就會顯示給收件者。

   ![顯示確認頁面介面的熒幕擷圖。](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [測試](create-lp.md#test-landing-page)和[發佈](create-lp.md#publish-landing-page)您的登陸頁面。

1. 建立[電子郵件](../email/create-email.md)傳遞，將流量引導至登陸頁面。

1. [將連結](../email/message-tracking.md#insert-links)插入您的訊息內容。 選取&#x200B;**[!UICONTROL 登陸頁面]**&#x200B;作為&#x200B;**[!UICONTROL 連結型別]**，然後選擇您建立的登陸頁面。

   ![顯示電子郵件連結插入介面的熒幕擷圖。](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >若要能夠傳送您的訊息，請確定您選取的登入頁面尚未過期。 [了解更多](create-lp.md#create-landing-page)

收到電子郵件後，如果您的收件者按一下登入頁面的連結並提交表單：

* 他們將被導向確認頁面。
* 將套用登陸頁面中定義的任何其他動作。 例如，使用者將會訂閱您的服務，或者他們不會再收到您的任何通訊。

以下是如何在不同的可能使用案例中使用[!DNL Adobe Campaign]登入頁面的一些範例。

## 設定檔贏取 {#lp-acquisition}

第一個範本可讓您新增或更新設定檔至Campaign資料庫。

1. 當[建立您的登入頁面](create-lp.md#create-landing-page)時，請選取&#x200B;**[!UICONTROL 贏取]**&#x200B;範本。

1. 在登入頁面屬性中，選取&#x200B;**[!UICONTROL 使用表單]**&#x200B;中參照的資料預先填入選項，以從設定檔預先載入任何現有資訊並避免建立重複專案。

1. 選取&#x200B;**[!UICONTROL 贏取]**&#x200B;頁面以編輯其內容。

1. 根據您要在設定檔上收集的資訊，視需要編輯文字欄位。

1. 新增核取方塊，邀請您的客戶訂閱您的Newsletter服務。 [瞭解如何建立服務](../audience/manage-services.md)

   ![熒幕擷圖顯示贏取頁面介面與電子報訂閱核取方塊。](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. 視需要調整您的內容並儲存變更。

1. 檢閱並[發佈](create-lp.md#publish-landing-page)您的登陸頁面。

1. 建立[電子郵件](../email/create-email.md)並[新增連結](../email/message-tracking.md#insert-links)至您的登入頁面。

收到電子郵件後，如果您的收件者按一下登入頁面的連結並提交表單，則會將其設定檔新增至Campaign資料庫，或更新其所提供的資訊。

![熒幕擷圖顯示Campaign資料庫中更新的設定檔。](assets/lp-uc-profile-updated.png){zoomable="yes"}

如果他們選擇接收您的Newsletter，他們將訂閱相應的服務。

![顯示電子報訂閱確認的熒幕擷圖。](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## 訂閱服務 {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="設定訂閱登陸頁面"
>abstract="訂閱頁面可讓您的客戶訂閱服務。"

最常見的使用案例之一，就是透過登入頁面，邀請您的客戶[訂閱服務](../audience/manage-services.md) （例如電子報或活動）。 請遵循下列步驟。

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. 為訂閱您的事件的使用者建立確認範本，以便您在建立服務時可以輕鬆選取它。 [了解更多](../audience/manage-services.md#create-confirmation-message)

   ![顯示確認電子郵件範本介面的熒幕擷圖。](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. 建立訂閱服務，儲存事件的註冊使用者。 [瞭解如何建立服務](../audience/manage-services.md)

1. 選取您建立的範本，作為使用者訂閱時將收到的確認電子郵件。

   ![顯示訂閱服務介面的熒幕擷圖。](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [建立登入頁面](create-lp.md#create-landing-page)，讓您的收件者註冊您的活動。 選取&#x200B;**[!UICONTROL 訂閱]**&#x200B;範本。

1. 選取&#x200B;**[!UICONTROL 訂閱]**&#x200B;頁面以編輯其內容。

1. 頁面內容隨即顯示。 選取與登入頁面表單相對應的部分，並展開&#x200B;**[!UICONTROL 核取方塊1]**&#x200B;區段。

1. 在&#x200B;**[!UICONTROL 訂閱與服務]**&#x200B;欄位中，選取您為事件建立的服務。 如果啟用&#x200B;**選項，請保留**&#x200B;訂閱狀態。

   ![顯示訂閱核取方塊介面的熒幕擷圖。](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. 視需要調整您的內容並儲存變更。

1. 檢閱並[發佈](create-lp.md#publish-landing-page)您的登陸頁面。

1. 建立[電子郵件](../email/create-email.md)及[新增連結](../email/message-tracking.md#insert-links)，以將流量引導至註冊登入頁面。

1. 設計電子郵件以宣佈您的活動已開放註冊。

收到電子郵件後，如果您的收件者按一下登入頁面的連結並提交表單，系統會將他們導向至確認頁面並新增至訂閱清單。

## 取消訂閱 {#lp-unsubscription}

您可以讓客戶使用登入頁面取消訂閱服務。

1. 為取消訂閱服務的使用者建立確認範本，以便您在建立服務時可以輕鬆選取它。 [了解更多](../audience/manage-services.md#create-confirmation-message)

1. 在您的[訂閱服務](../audience/manage-services.md)中，選取您建立的範本，作為使用者取消訂閱時將收到的確認電子郵件。

1. [建立登入頁面](create-lp.md#create-landing-page)。 選取&#x200B;**[!UICONTROL 取消訂閱]**&#x200B;範本。

1. 選取&#x200B;**[!UICONTROL 取消訂閱]**&#x200B;頁面以編輯其內容。

1. 頁面內容隨即顯示。 選取與登入頁面表單相對應的部分。

1. 新增&#x200B;**[!UICONTROL 核取方塊]**&#x200B;區段，選取服務，然後選取&#x200B;**[!UICONTROL 如果核取]**&#x200B;則取消訂閱選項。

   ![顯示取消訂閱核取方塊介面的熒幕擷圖。](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. 展開&#x200B;**[!UICONTROL 行動號召]**&#x200B;區段，並選取&#x200B;**[!UICONTROL 其他更新]**&#x200B;選項。 選取服務並核取&#x200B;**[!UICONTROL 選擇退出]**&#x200B;選項。

   ![熒幕擷圖顯示取消訂閱的call-to-action介面。](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. 視需要調整您的內容並儲存變更。

1. 檢閱並[發佈](create-lp.md#publish-landing-page)您的登陸頁面。

1. 建立[電子郵件](../email/create-email.md)並[新增連結](../email/message-tracking.md#insert-links)至登入頁面。

收到電子郵件後，如果您的收件者按一下登入頁面的連結並提交表單，系統會將他們導向至取消訂閱確認頁面，並從對應的訂閱服務中移除。

## 封鎖清單 {#lp-denylist}

法律規定必須讓收件者提供能夠取消訂閱來自品牌的通訊。 因此，您必須在每封寄送給收件者的電子郵件中一律包含&#x200B;**取消訂閱連結**。 按一下此連結後，收件者會被導向包含確認選擇退出按鈕的登陸頁面。

您可以設定&#x200B;**[!UICONTROL 封鎖清單]**&#x200B;登陸頁面，讓使用者可以選擇退出所有傳遞。

1. 當[建立您的登入頁面](create-lp.md#create-landing-page)時，請選取&#x200B;**[!UICONTROL 封鎖清單]**&#x200B;範本。

1. 選取&#x200B;**[!UICONTROL 封鎖清單]**&#x200B;頁面以編輯其內容。

1. 展開&#x200B;**[!UICONTROL 行動號召]**&#x200B;區段，並選取&#x200B;**[!UICONTROL 其他更新]**&#x200B;選項。

1. 從對應的下拉式清單中選取&#x200B;**[!UICONTROL 管道（電子郵件）]**，讓您的收件者僅能選擇退出電子郵件通訊。 您也可以選取&#x200B;**[!UICONTROL 依所有通道]**，以選擇退出所有通道上的所有通訊。

   ![熒幕擷圖顯示封鎖清單call-to-action介面。](assets/lp-uc-denylist.png){zoomable="yes"}

1. 視需要調整您的內容並儲存變更。

1. 檢閱並[發佈](create-lp.md#publish-landing-page)您的登陸頁面。

1. 建立[電子郵件](../email/create-email.md)並[將連結](../email/message-tracking.md#insert-links)新增至您的登陸頁面，讓使用者選擇退出接收通訊。

收到電子郵件後，如果您的收件者按一下登入頁面的連結並提交表單，系統會將他們導向封鎖清單確認頁面，且他們的設定檔會更新為所提供的資訊。

若要檢查對應的設定檔選擇是否已更新，請瀏覽至&#x200B;**[!UICONTROL 設定檔]**&#x200B;功能表並選取該設定檔。

例如，如果您選擇更新登陸頁面中的&#x200B;**[!UICONTROL 頻道（電子郵件）]**&#x200B;選項，則會核取&#x200B;**[!UICONTROL 不再透過電子郵件聯絡]**&#x200B;選項。

![熒幕擷圖顯示已使用封鎖清單偏好設定更新的設定檔。](assets/lp-uc-denylist-profile.png){zoomable="yes"}

除非再次訂閱，否則此設定檔將不會收到您品牌的電子郵件通訊。