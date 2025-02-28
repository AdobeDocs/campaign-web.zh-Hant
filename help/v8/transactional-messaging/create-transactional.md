---
audience: end-user
title: 建立異動訊息
description: 瞭解如何在Campaign網頁使用者介面中建立交易式訊息
exl-id: 74e468f5-d9c3-4470-8ff2-68648b5f396f
source-git-commit: 7185e1cbc8ce9dd325bebc20c0ac362d7067f3e9
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 20%

---

# 建立異動訊息

在交易式訊息中，事件會觸發個人化訊息的傳送。
若要啟用此功能，您必須為每個事件型別建立訊息範本。 這些範本包含個人化交易式訊息的所有必要資訊。

## 建立異動訊息範本 {#transactional-template}

在Campaign Web使用者介面中，交易式訊息設定的第一步是建立範本或直接建立訊息。 這與使用者端主控台](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional)上的[異動訊息組態不同。

交易式訊息範本可用於在設定檔收到的傳送內容到達最終對象之前進行預覽。 例如，管理員可以設定並設定範本，讓行銷使用者可以隨時使用。

若要建立異動訊息範本，請遵循下列步驟：

* 在&#x200B;**[!UICONTROL 觸發訊息]**&#x200B;區段中，移至&#x200B;**[!UICONTROL 異動訊息]**。 在&#x200B;**[!UICONTROL 範本]**&#x200B;標籤中，您可以看到異動訊息的所有傳遞範本。 按一下&#x200B;**[!UICONTROL 建立異動訊息範本]**&#x200B;按鈕，開始建立範本。

  ![](assets/transactional-templates.png){zoomable="yes"}

* 在顯示的新頁面中，選擇範本的頻道。 例如，我們選取&#x200B;**[!UICONTROL 電子郵件]**&#x200B;頻道。 您也可以從其他訊息範本中工作，並在範本清單中選取它。

  ![](assets/transactional-template-channel.png){zoomable="yes"}

  再按一下&#x200B;**[!UICONTROL 建立交易式訊息]**&#x200B;按鈕，以驗證在選取的頻道上建立範本。

* 您現在可以存取交易式訊息範本的設定。

  ![](assets/transactional-template-configuration.png){zoomable="yes"}

### 交易型訊息屬性 {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="交易型傳訊屬性"
>abstract="填寫此表單以設定交易型傳訊屬性"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="交易型傳訊電子郵件屬性"
>abstract="填寫此表單以設定交易型傳訊電子郵件屬性"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="交易型傳訊 SMS 屬性"
>abstract="填寫此表單以設定交易型傳訊 SMS 屬性"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="交易型傳訊推播屬性"
>abstract="填寫此表單以設定交易型傳訊推播屬性"

交易式訊息的&#x200B;**[!UICONTROL 屬性]**&#x200B;區段將協助您設定：

* **[!UICONTROL 標籤]**&#x200B;是顯示在交易式訊息清單中的名稱。 明確說明以供研究和未來使用。
* **[!UICONTROL 內部名稱]**&#x200B;是唯一的名稱，可將您的訊息與其他建立的訊息區分開來。
* **[!UICONTROL 資料夾]**&#x200B;是建立交易式訊息範本的位置。
* **[!UICONTROL Execution資料夾]**&#x200B;是郵件在執行後儲存的位置。
* **[!UICONTROL 傳遞代碼]**：視需要協助辨識訊息以供報告的代碼。
* **[!UICONTROL 描述]**
* **[!UICONTROL Nature]**&#x200B;是您傳送的性質，列於列舉&#x200B;*deliveryNature*&#x200B;中。 [進一步瞭解分項清單](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations)

![](assets/template-properties.png){zoomable="yes"}

### 行動應用程式 {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="交易型傳訊行動應用程式"
>abstract="在此區段，您可以選取要推播訊息的應用程式。"

在此區段，您可以選取要推播訊息的應用程式。

按一下「重新搜尋」圖示，即可存取Adobe Campaign例項中列出的行動應用程式。

![](assets/transactional-mobileapp.png){zoomable="yes"}

### 情境範例 {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="交易型傳訊情境"
>abstract="情境範例可讓您建立測試事件，以預覽使用客戶設定檔個人化接收的交易型訊息。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="交易型傳訊情境"
>abstract="情境範例可讓您建立測試事件，以預覽使用客戶設定檔個人化接收的交易型訊息。 "

情境範例可讓您建立測試事件，以預覽使用客戶設定檔個人化接收的交易型訊息。

此步驟為選填。您可以使用沒有上下文範例的範本，但缺點在於您無法預覽個人化內容。

在設定密碼的範例中，事件會傳送使用者的名字、姓氏和個人化連結以重設密碼。 可以設定上下文，如下所示。

內容的內容取決於您需要的個人化。

![](assets/transactional-context.png){zoomable="yes"}

### 交易型訊息範本內容 {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="交易型傳訊內容"
>abstract="了解如何建立交易型傳訊內容"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="交易型傳訊個人化"
>abstract="了解如何建立個人化交易型傳訊內容"

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_event_context"
>title="事件內容"
>abstract="此選單提供來自觸發事件的變數，您可以利用這些變數個人化您的交易訊息內容。"

處理交易式訊息的內容，就像建立傳送的內容一樣。 按一下&#x200B;**[!UICONTROL 開啟電子郵件設計工具]**&#x200B;或&#x200B;**[!UICONTROL 編輯電子郵件內文]**，然後選取範本內容或匯入您的HTML程式碼。

![](assets/template-content.png){zoomable="yes"}

若要在內容中新增個人化，請按一下要新增該個人化的區段，然後選擇&#x200B;**[!UICONTROL 新增Personalization]**&#x200B;圖示。

![](assets/template-perso.png){zoomable="yes"}

您將可以存取&#x200B;**[!UICONTROL 編輯個人化]**視窗。
若要從觸發程式事件新增變數，請按一下**[!UICONTROL 事件內容]**&#x200B;圖示。 您可以瀏覽您為範本定義的前後關聯（[深入瞭解前後關聯](#context-sample)），然後按一下&#x200B;**[!UICONTROL +]**&#x200B;按鈕以插入所需的變數。

您可以在下圖中看到如何新增個人化的名字。

![](assets/template-firstname.png){zoomable="yes"}

在我們的範例中，我們會新增名字、姓氏，並個人化&#x200B;**[!UICONTROL 重設您的密碼]**&#x200B;按鈕連結。

![](assets/template-button.png){zoomable="yes"}

### 預覽您的範本

在範本建立的這個階段，您可能想要預覽範本內容，並檢查個人化。

若要這麼做，請填入[內容範例](#context-sample)，然後按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕。

![](assets/template-preview.png){zoomable="yes"}

## 建立交易型訊息 {#transactional-message}

您可以直接或使用交易式訊息範本建立交易式訊息。 [瞭解如何建立異動訊息範本](#transactional-template)。

若要建立交易式訊息，請遵循下列步驟：

* 在&#x200B;**[!UICONTROL 觸發訊息]**&#x200B;區段中，移至&#x200B;**[!UICONTROL 異動訊息]**。 在&#x200B;**[!UICONTROL 瀏覽]**&#x200B;標籤中，您可以看到所有建立的交易式訊息。 按一下&#x200B;**[!UICONTROL 建立交易式訊息]**&#x200B;按鈕，開始建立您的訊息。

  ![](assets/transactional-browse.png){zoomable="yes"}

* 在顯示的新頁面中，選擇訊息的頻道，並選擇要使用的範本。 在我們的範例中，我們選擇[我們在這裡建立的範本](#transactional-template)。

  ![](assets/transactional-channel.png){zoomable="yes"}

  再次按一下&#x200B;**[!UICONTROL 建立交易式訊息]**&#x200B;按鈕，以驗證在選取的頻道上建立您的訊息。

* 您現在可以存取交易式訊息的設定。 您的訊息會繼承範本的設定。 此頁面與異動訊息範本設定頁面幾乎相同，不同之處在於此頁面也包含事件型別設定。

  ![](assets/transactional-configuration.png){zoomable="yes"}

  將訊息的設定填寫為範本：
   * [異動訊息屬性](#transactional-properties)
   * [內容範例](#context-sample)
   * [訊息內容](#transactional-content)
和[設定事件型別](#event-type)，如下所述。

* 在[驗證您的交易式訊息](validate-transactional.md)之後，按一下&#x200B;**[!UICONTROL 檢閱並發佈]**按鈕以建立並發佈您的訊息。
觸發器現在可以推送交易式訊息的傳送。

### 關於事件類型 {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="交易型傳訊事件"
>abstract="事件類型的設定會將訊息連結至觸發事件。"

事件類型的設定會將訊息連結至觸發事件。

在Campaign Web使用者介面中，您可以選取和已建立的事件型別，或直接在此設定頁面中建立您的事件型別。

![](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>如果您選取另一個交易式訊息目前正在使用的事件型別，則會觸發這兩個訊息。 為求最佳實務，**強烈建議將ONE事件型別連結至ONE交易式訊息。**

## 將優惠方案新增至交易式訊息 {#transactional-offers}

您可以選擇將優惠方案納入交易式訊息，讓您向一般使用者呈現相關提案，即使訊息是由事件觸發亦然。

此功能可在交易式訊息的內容編輯階段存取。 只需按一下&#x200B;**[!UICONTROL 設定優惠方案]**&#x200B;按鈕即可進行設定。

設定程式與設定標準傳送的優惠方案相同。 [瞭解如何新增優惠方案至您的訊息](../msg/offers.md)。

![](assets/transactional-offers.png){zoomable="yes"}
