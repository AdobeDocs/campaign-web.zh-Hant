---
audience: end-user
title: 探索介面
description: Campaign v8 Web 使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: 86a343aae763e753bc63ca2cab3c22cda07d7c16
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 100%

---

# 探索介面 {#user-interface}

新的 Campaign v8 Web 介面提供了現代直覺的使用者體驗，可簡化行銷活動的設計和傳遞。這個新介面整合 Adobe Experience Cloud 應用程式和解決方案。


>[!NOTE]
>
>本文件會經常更新以反映產品使用者介面最近的變更。不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。


## 左側導覽功能表 {#user-interface-left-nav}

瀏覽左側連結可存取 Campaign v8 Web 功能。幾個連結會顯示可以排序和篩選的物件清單。您也可以設定欄以顯示所有您需要的資訊。請參閱本[章節](#list-screens)。有些清單畫面部分為唯讀。左側導覽功能表與清單中顯示的項目取決於您的使用者權限。若要了解權限的詳細資訊，請參閱[本章節](permissions.md)。

![](assets/home.png)

### 首頁 {#user-interface-home}

此畫面包含快速存取主要 Campaign v8 Web 功能的重要連結和資源。

「**最近項目**」清單提供最近建立和修改之傳遞的快速鍵。此清單會顯示其管道、狀態、所有者、建立與修改日期。

「**關鍵績效指標**」可讓您使用常見的 KPI 值來檢查平台的服務效率。在[本頁面](../reporting/kpis.md)中進一步瞭解這些 KPI。

從首頁的&#x200B;**學習**&#x200B;章節存取 Campaign v8 Web 重要說明頁面。

### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;選單會顯示所有 Campaign 元件以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽所有 Campaign v8 元件、資料夾和方案，檢查相關聯的權限，並從此選單建立資料夾和子資料夾。"

「**探索工具**」選單會顯示所有 Campaign 資源以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽您所有的 Campaign v8 元件、資料夾和結構描述，並建立傳遞、工作流程和行銷活動。

「**探索工具**」中顯示的項目取決於您的使用者權限。如果有適當的權限，您也可以新增資料夾和子資料夾。若要了解權限的詳細資訊，請參閱[本章節](permissions.md)。

您可以設定欄來自訂顯示，以便檢視您需要的所有資訊。請參閱本[章節](#list-screens)。您也可以新增資料夾和子資料夾，請參閱[本章節](permissions.md#folders)以取得詳細資訊。

如需 Campaign 探索工具、資料夾階層和資源的詳細資訊，請參閱此 [Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}。

### 行銷活動管理 {#user-interface-campaign-management}

在「行銷活動管理」區段中，您可以存取行銷活動、傳遞以及工作流程。

* **行銷活動** - 這是您的行銷活動清單以及行銷活動範本。預設情況下，您可以針對每個行銷活動檢視開始/結束/建立/最後修改日期、目前狀態以及建立該活動之行銷活動操作人員的姓名。您可以依狀態、開始/結束日期、資料夾篩選清單，或建立進階篩選以定義您自己的篩選標準。若要了解行銷活動的詳細資訊，請參閱[本章節](../campaigns/gs-campaigns.md)。

* **傳遞** - 瀏覽您的傳遞清單。依預設，您可以檢視其狀態、最後修改日期，以及 KPI。您可以依狀態、聯絡日期或管道篩選清單。按一下電子郵件傳遞來開啟其儀表板以取得傳遞詳細資料概觀。其他管道上的傳遞是唯讀的。若要了解傳遞的詳細資訊，請參閱[本章節](../msg/gs-messages.md)。

  使用「**更多動作**」按鈕來刪除或複製傳遞。

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流程** - 在此畫面中，您可以存取工作流程和工作流程範本的完整清單。您可以檢查其狀態、上次/下次執行日期，並建立新的工作流程或新的工作流程範本。您可以使用和其他物件相同的標準篩選清單。此外，您可以篩選工作流程，無論其是否屬於行銷活動。若要了解工作流程的詳細資訊，請參閱[本章節](../workflows/gs-workflows.md)。


### 客戶管理 {#user-interface-customer-management}

在「客戶管理」章節中，您可以檢視您的收件者、對象和訂閱。這些是唯讀清單。

* **收件者** - 存取您的收件者資料庫。依預設，您可以檢視其電子郵件地址、名字和姓氏。若要了解收件者的詳細資訊，請參閱[本章節](../audience/about-recipients.md)。
* **對象** - 這是您的對象清單。依預設，您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依據來源篩選清單。若要了解對象與清單的詳細資訊，請參閱[本章節](../audience/about-recipients.md)。
* **訂閱** - 瀏覽您的訂閱清單。預設情況下，您可以檢視其類型、模式和標籤。若要了解如何管理訂閱和取消訂閱，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}。

### 決策管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="優惠"
>abstract="瀏覽已使用「**互動**」模組在主控台中建立的優惠清單和優惠範本。這些是唯讀清單。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="將優惠新增到傳遞"

在「決策管理」部分，您可以檢視優惠和優惠範本。這些是唯讀清單。

* **優惠** - 瀏覽透過使用「**互動**」模組在主控台建立的優惠清單和優惠範本。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。

若要了解如何在電子郵件和簡訊中建立和傳送優惠，請參閱[本章節](../content/offers.md)。

## 頂端列 {#top-bar}

使用介面的頂端列進行以下作業：

* 以 Beta 測試人員身份分享您的意見回饋
* 在組織和實例之間切換
* 在 Adobe Experience Cloud 應用程式之間切換
* 存取說明頁面、聯絡支援人員和分享意見回饋。您可以從搜尋欄位搜尋說明文章和影片。

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->


## 內容說明 {#user-interface-help}

介面中會提供內容關聯式說明。若有提供，請按一下 `?` 圖示以顯示說明資訊和相關文件的連結。

![](assets/context-help.png){width="40%" align="left"}

在新的 Beta 版本中，嵌入內容說明中的 **AI 驅動的知識助理**&#x200B;可輕鬆篩選大量文件存放庫，並立即找出所需的精確資訊，為文件搜尋和回答操作方法問題方面帶來了全面革新。

透過 Campaign Gen AI 的功能，此助理將改變您的體驗，讓資訊檢索和問題解決變得輕而易舉。無論您是在複雜任務中尋求指引，還是導覽大量文件，AI 驅動的知識助理都是您的終極夥伴，在每次互動中提供無與倫比的效率和準確性。

若要了解詳細資訊，請參閱[本章節](using-ai.md)。

## 支援的瀏覽器 {#browsers}

Campaign v8 Web 目的是要在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中以最佳方式運作。您可能無法在舊版本或其他瀏覽器上使用某些功能。

## 語言偏好設定 {#language-pref}

Campaign v8 Web 目前提供以下語言版本：

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


您對 Campaign Web 的預設語言是由使用者設定檔中指定的偏好語言所決定。那與您的 Campaign 伺服器和用戶端主控台的語言無關。

若要變更您的語言：

1. 按一下右上角您的設定檔圖示，然後選取「**偏好設定**」。
1. 然後，按一下您電子郵件地址下顯示的語言連結。
1. 選取您偏好的語言，然後按一下「**儲存**」。您可以選取第二語言，以防您使用的元件沒有您第一語言的版本。

## 深色主題 {#dark-theme}

您可以從個人資料圖示切換到深色主題。使用「**深色主題**」切換以啟用/停用。

## 了解更多 {#learn-more}

了解如何瀏覽、搜尋和篩選 Campaign 環境中的可用清單 ([在此頁面](list-filters.md))。


<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球報告傳送"
>abstract="此畫面中會顯示追蹤報告指標"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球報告追蹤"
>abstract="此畫面中會顯示追蹤報告指標"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="活動中的工作流程清單"
>abstract="活動中的工作流程清單"

<!-- delivery settings-->


