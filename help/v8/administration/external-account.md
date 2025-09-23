---
title: 管理外部帳戶
description: 瞭解如何設定外部帳戶
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# 促銷活動特定外部帳戶 {#external-account}

請依照下列步驟，根據您選取的外部帳戶型別進行帳戶設定。

## 退回郵件 (POP3) {#bounce}

「退回郵件」外部帳戶指定用來連線至電子郵件服務的外部POP3帳戶。 所有設定為POP3存取的伺服器都可以接收傳回郵件。

![熒幕擷圖顯示[退回郵件(POP3)]外部帳戶設定欄位。](assets/external_account_bounce.png)

若要設定&#x200B;**[!UICONTROL 退回郵件(POP3)]**&#x200B;外部帳戶，請填寫下列欄位：

* **[!UICONTROL 伺服器]** - POP3伺服器的URL。

* **[!UICONTROL 連線埠]** - POP3連線埠號碼（預設連線埠為110）。

* **[!UICONTROL 帳戶]** — 使用者名稱。

* **[!UICONTROL 密碼]** — 使用者帳戶密碼。

* **[!UICONTROL 加密]** — 選擇的加密型別，包括：
   * 依預設（若連線埠110則為POP3，若連線埠995則為POP3）。
   * 傳送STARTTLS後切換至SSL的POP3。
   * POP3不安全（預設連線埠110）。
   * POP3安全於SSL之上（預設連線埠995）。

* **[!UICONTROL 函式]** — 選取&#x200B;**[!UICONTROL 傳入電子郵件]**&#x200B;設定接收傳入電子郵件的帳戶，或選取&#x200B;**[!UICONTROL SOAP路由器]**&#x200B;處理SOAP要求。

>[!IMPORTANT]
>
>使用Microsoft OAuth 2.0設定POP3外部帳戶之前，您必須先在Azure入口網站中註冊應用程式。 如需詳細資訊，請參閱[此頁面](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}。

若要使用Microsoft OAuth 2.0設定POP3外部連結，請核取Microsoft OAuth 2.0選項並填寫下列欄位：

* **[!UICONTROL Azure租使用者]**

  Azure ID (或目錄（租使用者） ID)可在Azure入口網站應用程式概觀的Essentials下拉式清單中找到。

* **[!UICONTROL Azure使用者端ID]**

  使用者端ID (或應用程式（使用者端） ID)可在Azure入口網站應用程式概觀的Essentials下拉式清單中找到。

* **[!UICONTROL Azure使用者端密碼]**

  使用者端密碼識別碼可在Azure入口網站應用程式的「憑證和密碼」功能表的「使用者端密碼」欄中找到。

* **[!UICONTROL Azure重新導向URL]**

  您可在Azure入口網站中的應用程式驗證功能表中找到重新導向URL。 它應該以下列語法nl/jsp/oauth.jsp結尾，例如`https://redirect.adobe.net/nl/jsp/oauth.jsp`。

安裝及使用使用者端主控台中的[測試連線]按鈕需要網際網路存取。 設定完成後，inMail程式便可在沒有網際網路的情況下與Microsoft伺服器通訊。

輸入不同的認證後，您可以按一下「設定連線」以完成外部帳戶設定。

## 路由 {#routing}

若要設定外部傳遞的特定外部帳戶，請遵循下列步驟。

1. 建立外部帳戶。 [了解更多](create-external-account.md)

1. 選取&#x200B;**[!UICONTROL 路由]**&#x200B;型別。

   ![顯示路由外部帳戶型別選擇的熒幕擷圖。](assets/external-account-routing.png){zoomable="yes"}

1. 選取想要的頻道，然後按一下&#x200B;**[!UICONTROL 建立]**。

1. 在外部帳戶&#x200B;**[!UICONTROL 詳細資料]**&#x200B;區段中，預設會選取&#x200B;**[!UICONTROL 外部]**&#x200B;作為&#x200B;**[!UICONTROL 傳遞模式]**。

   ![熒幕擷圖顯示路由外部帳戶的傳遞模式設定。](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >目前，**[!UICONTROL 外部]**&#x200B;是唯一可用的模式。

1. 若要在傳遞執行後處理流程，請將此外部化至後處理工作流程。 使用[外部訊號](../workflows/activities/external-signal.md)活動建立工作流程，並從&#x200B;**[!UICONTROL 後續處理]**&#x200B;欄位中選取它。

   ![顯示路由外部帳戶後處理欄位設定的熒幕擷圖。](assets/external-account-post-processing.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 活動]**&#x200B;欄位中，編輯記錄中顯示的後處理工作流程活動的名稱。<!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## 執行執行個體 {#instance-exec}

如果您有分段的架構，請識別與控制執行個體相關聯的執行個體，並建立它們之間的連線。 在執行例項上部署異動訊息範本。

![顯示執行執行個體外部帳戶設定欄位的熒幕擷圖。](assets/external_account_exec.png)

若要設定&#x200B;**[!UICONTROL 執行例項]**&#x200B;外部帳戶：

* **[!UICONTROL URL]** — 安裝執行個體的伺服器的URL。

* **[!UICONTROL 帳戶]** — 帳戶的名稱，符合操作員資料夾中定義的訊息中心代理程式。

* **[!UICONTROL 密碼]** — 運運算元資料夾中定義的帳戶密碼。

* **[!UICONTROL 方法]** — 在Web服務或同盟資料存取(FDA)之間選擇。

  針對FDA，請選取您的FDA帳戶。 請注意，與外部系統的Campaign連線僅限於進階使用者，而且只能從使用者端主控台使用。 [了解更多](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL 建立封存工作流程]** — 對於在訊息中心中註冊的每個執行執行個體，無論您是否有一或多個執行個體，請為與該執行個體相關聯的每個外部帳戶建立個別的封存工作流程。
