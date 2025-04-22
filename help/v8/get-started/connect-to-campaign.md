---
title: 連線至 Adobe Campaign Web 介面
description: 了解如何連線至 Adobe Campaign Web 使用者介面
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: ht
source-wordcount: '884'
ht-degree: 100%

---

# 連線至 Adobe Campaign {#connect-to-campaign}

Experience Cloud 是 Adobe 的整合式數位行銷應用程式、產品和服務系列。您可以從其直覺式介面，快速存取雲端應用程式、產品功能和服務。閱讀此頁面，了解如何連線至 Adobe Experience Cloud，以及存取 Adobe Campaign Web 介面。

## 登入 Adobe Experience Cloud {#sign-in-to-exc}

您只能使用單一登入 (SSO) 來連線至 Campaign。通常 Experience Cloud 管理員會授予存取應用程式和服務的權限。 依照電子郵件邀請中的步驟進行，加入 Experience Cloud。

若要登入 Adobe Experience Cloud，請按照以下基本步驟：

1. 瀏覽至 [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。

1. 使用 Adobe ID 或 Enterprise ID 登入。若要了解更多關於 Adobe 身分類型的資訊，請參閱[此文章](https://helpx.adobe.com/tw/enterprise/using/identity.html){target="_blank"}。

   登入 Experience Cloud 後，您便可以快速存取您的所有解決方案和應用程式。

   ![顯示 Adobe Experience Cloud 首頁的螢幕擷圖](assets/exc-home.png){zoomable="yes"}

1. 確認您位於正確的組織。

   ![顯示 Adobe Experience Cloud 中組織選取的螢幕擷圖](assets/exc-orgs.png){zoomable="yes"}{width="50%" align="left"}

   若要了解更多關於 Adobe Experience Cloud 中組織的資訊，請參閱[此文章](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=zh-hant){target="_blank"}。

## 存取 Adobe Campaign {#access-to-campaign}

若要存取 Campaign 環境，請從 Adobe Experience Cloud 首頁的「**快速存取**」區段中，選取 **Campaign**。

如果您已經連線至另一個 Adobe Experience Cloud 解決方案，從螢幕右上角的解決方案切換器瀏覽至您的 Campaign 環境。

![顯示 Adobe Experience Cloud 中解決方案切換器的螢幕擷圖](assets/solution-switcher.png){zoomable="yes"}

如果您擁有多個環境的存取權，包括 Campaign 控制面板，請按一下正確執行個體的「**啟動**」按鈕。

![顯示 Adobe Campaign 啟動按鈕的螢幕擷圖](assets/launch-campaign.png){zoomable="yes"}

您現在已連接到 Campaign。如需了解如何開始使用使用者介面，請參閱[此頁面](user-interface.md)。

### 存取控制 {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，您才能建立此物件。"

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="此對象為唯讀"
>abstract="您沒有編輯此對象的權限。如果需要，請聯絡管理員為您授予存取權。"

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="此服務為唯讀資料"
>abstract="您沒有編輯此服務的權限。如果需要，請聯絡管理員為您授予存取權。"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="收件者唯讀設定檔"
>abstract="您沒有編輯此輪廓的權限。如果需要，請聯絡管理員為您授予存取權。"

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="此行銷活動為唯讀資料"
>abstract="您沒有編輯此行銷活動的權限。如果需要，請聯絡管理員為您授予存取權。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="此傳遞為唯讀資料"
>abstract="您沒有編輯此傳遞的權限。如果需要，請聯絡管理員為您授予存取權。"

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="此工作流程為唯讀資料"
>abstract="您沒有編輯此工作流程的權限。如果需要，請聯絡管理員為您授予存取權。"

存取控制會限制存取主要清單中的物件和資料，例如傳遞、收件者或工作流程。這些限制也適用於「探索工具」導覽樹狀結構。此外，您需要從使用者介面建立、刪除、複製和編輯物件的權限。

Campaign Web 中的所有權限都會與 Campaign 用戶端主控台權限進行同步。只有 Campaign 管理員可以定義和修改使用者權限。

在瀏覽 Campaign Web 使用者介面時，您可以根據自己的權限存取資料、物件和功能。例如，如果沒有資料夾的存取權限，就看不到。您的權限也會影響物件和資料管理。如果沒有特定資料夾的寫入權限，即使可以在使用者介面中看到，也無法在該資料夾中建立傳遞。

您可以[在這裡了解如何檢視和管理權限](permissions.md)。

## Adobe Experience Cloud 頂端導覽 {#top-bar}

瀏覽介面的頂端列以進行下列作業：

* 提供有關 Campaign Web 使用者介面的意見回饋。
* 切換至不同的組織。
* 切換至您不同的 Adobe Experience Cloud 解決方案與應用程式。
* 在 [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=zh-hant){target="_blank"} 上搜尋說明。
* 查看您的產品通知。
* 編輯您的 Adobe 設定檔及管理各項設定，例如[更新您最愛的語言](#language-pref)或[切換為淺色/深色主題](#dark-theme)。

![顯示 Adobe Experience Cloud 頂端導覽列的螢幕擷圖](assets/do-not-localize/unified-shell.png){zoomable="yes"}{width="50%" align="left"}

## 支援的瀏覽器 {#browsers}

Adobe Campaign Web 目的是要在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中以最佳方式運作。您在舊版本或其他瀏覽器上使用某些功能時可能會遇到問題。

## 語言偏好設定 {#language-pref}

Adobe Campaign Web 目前提供以下語言版本：

* 英文 (US) - EN-US
* 法文 - FR
* 德文 - DE
* 義大利文 - IT
* 西班牙文 - ES
* 葡萄牙文 (巴西) - PTBR
* 日文 - JP
* 韓文 - KR
* 簡體中文 - CHS
* 繁體中文 - CHT

Campaign Web 的預設語言是由您的使用者個人檔案中指定的偏好語言所決定。那與您的 Campaign 伺服器和用戶端控制台的語言無關。

若要變更您的語言：

1. 按一下右上角您的個人檔案圖示，然後選取「**偏好設定**」。
1. 按一下您電子郵件下方顯示的語言連結。
1. 選取您偏好的語言，然後按一下「**儲存**」。您可以選取第二語言，以防您使用的元件沒有您第一語言的版本。


## 深色和淺色主題 {#dark-theme}

Adobe Campaign 提供淺色和深色主題。依據預設，使用者介面會在淺色主題中啟用。若要切換至深色主題，請按一下設定檔圖示，然後使用&#x200B;**深色主題**&#x200B;切換開關來啟用或停用。

使用者設定檔設定及帳戶偏好的詳細資訊，請參閱[此區段](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=zh-hant#preferences){target="_blank"}。

若要了解更多關於 Experience Cloud 中央介面元件的資訊，請參閱[此文件](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=zh-hant){target="_blank"}。