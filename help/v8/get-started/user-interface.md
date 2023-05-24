---
audience: end-user
title: 探索介面
description: Campaign v8 Web 使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
source-git-commit: 25082a853fb095c24d7c22d00310992ac4e97be9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 探索介面 {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="探索介面"
>abstract="新的 Campaign v8 Web 介面提供了整合、直覺和一致的使用者體驗。"

新的 Campaign v8 Web 介面提供了現代直覺的使用者體驗，可簡化行銷活動的設計和傳遞。這個新介面與 Adobe Experience Platform 整合在一起。

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>本文件會經常更新以反映產品使用者介面最近的變更。不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左側導覽選單

瀏覽左側連結可存取 Campaign v8 Web 功能。幾個連結會顯示可以排序和篩選的物件清單。您也可以設定欄以顯示所有您需要的資訊。請參閱本[章節](#list-screens)。所有清單都是唯讀的，電子郵件傳遞清單表除外。按一下清單項目以編輯/檢視的這個功能在 Alpha 版本未提供。在未來的版本，所有清單將可編輯。左側導覽選單顯示的項目取決於您的使用者權限。

![](assets/home.png)

### 首頁

此畫面包含快速存取主要 Campaign v8 Web 功能的重要連結和資源。「**最近項目**」清單提供最近建立和修改之傳遞的快速鍵。此清單顯示其建立和修改日期與狀態。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

從首面下方區段存取 Campaign v8 Web 重要說明頁面。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### 總管

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="總管"
>abstract="**總管**&#x200B;選單顯示與用戶端主控台相同的資料夾階層結構。瀏覽所有 Campaign v8 元件、資料夾和綱要。所有清單都是唯讀的，電子郵件傳遞清單表除外。"

**總管**&#x200B;選單顯示與用戶端主控台相同的資料夾階層結構。瀏覽所有 Campaign v8 元件、資料夾和綱要。所有清單都是唯讀的，電子郵件傳遞清單表除外。

總管中顯示的項目取決於您的使用者權限。

如同任何清單畫面，您可以設定欄來個人化顯示以檢視所有您需要的資訊。請參閱本[章節](#list-screens)。

如需 Campaign 總管的詳細資訊，請參閱本[文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}。
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### 行銷活動管理

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="行銷活動"
>abstract="這是您的行銷活動清單。您可以檢視有用的資訊，例如其開始/結束/最後修改日期，以及其狀態。您可以依狀態或開始/結束日期篩選清單。按一下「建立行銷活動」按鈕以新增行銷活動。 選取行銷活動以檢視其內容、傳遞和詳細資訊。 瀏覽至「範本」標籤以檢視和建立範本。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="傳遞"
>abstract="瀏覽您的傳遞清單。您可以檢視其狀態、聯絡人及修改日期、關鍵KPI。 您可以依狀態、聯絡日期或管道篩選清單。按一下「建立傳遞」按鈕以新增傳遞。 選取傳遞以檢視其內容、對象和詳細資訊。"

* **行銷活動** - 這是您的行銷活動清單。依預設，您可以檢視其開始/結束/最後修改日期，以及其狀態。您可以依狀態或開始/結束日期篩選清單。也提供行銷活動範本。這些清單是唯讀的。

* **傳遞** - 瀏覽您的傳遞清單。依預設，您可以檢視其狀態、最後修改日期，以及 KPI。您可以依狀態、聯絡日期或管道篩選清單。按一下電子郵件傳遞來開啟其儀表板以取得傳遞詳細資料概觀。其他管道上的傳遞是唯讀的。傳遞範本也是唯讀模式。您可以使用用戶端主控台來編輯它們。請參閱本[文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}。

   使用「**更多動作**」按鈕來刪除或複製傳遞。

   ![](assets/more-actions.png){width="70%" align="left"}

### 客戶管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="收件者"
>abstract="存取您的收件者資料庫。您可以檢視有用的資訊，例如其電子郵件地址、名字和姓氏。此清單是唯讀的。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="對象"
>abstract="這是您的對象清單。您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依來源來篩選清單。此清單是唯讀的。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="訂閱清單"
>abstract="瀏覽您的訂閱清單。您可以檢視其類型、模式和標籤。此清單是唯讀的。"

* **收件者** - 存取您的收件者資料庫。依預設，您可以檢視其電子郵件地址、名字和姓氏。此清單是唯讀的。
* **對象** - 這是您的對象清單。依預設，您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依來源來篩選清單。此清單是唯讀的。
* **訂閱清單** - 瀏覽您的訂閱清單。依預設，您可以檢視其類型、模式和標籤。此清單是唯讀的。
* **目標定位工作流程** - 存取您的行銷活動工作流程清單。依預設，您可以檢視其狀態、上次/下次處理日期和環境。您可以依狀態、上次處理日期和工作流程類型來篩選清單。也提供工作流程範本。這些清單是唯讀的。

### 決策管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="優惠"
>abstract="瀏覽您的互動優惠清單。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。這些清單是唯讀的。"

* **優惠** - 覽您的互動優惠清單。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。這些清單是唯讀的。

## 頂端列

介面的頂端列可讓您：

* 以 Alpha 測試人員身份分享您的意見回饋
* 在組織和實例之間切換
* 在 Adobe Experience Cloud 應用程式之間切換
* 存取說明頁面、聯絡支援人員和分享意見回饋。您可以從搜尋欄位搜尋說明文章和影片。

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 設定清單畫面 {#list-screens}

左側導覽選單中的幾個連結 (例如 **傳遞**&#x200B;或&#x200B;**行銷活動**) 會顯示物件清單。這些清單畫面都是唯讀的，電子郵件傳遞清單除外。

若要更快地找到項目，您可以使用搜尋列或根據內容關聯式條件篩選清單。

![](assets/filter.png){width="70%" align="left"}

清單顯示在欄中。您可以變更欄設定來顯示其他資訊。為此，按一下清單右上角的圖示。您可以新增或移除欄並變更其顯示順序。

![](assets/columns.png){width="70%" align="left"}

您可以按一下任何欄標題來排序清單中的項目。會顯示箭頭 (向上或向下) 表示清單已按該欄排序。對於數字或日期欄，向上箭頭表示清單按遞增順序排序，而向下箭頭表示遞減順序。對於字串或英數字元欄，值按字母順序列出。

## 內容關聯式說明和入門指南

介面中提供內容關聯式說明。可用時，按一下 **?**&#x200B;圖示可顯示說明資訊和相關文件連結。

![](assets/context-help.png){width="70%" align="left"}

也提供入門指南，可協助您開始使用 Campaign v8 Web。按一下右下角的圖示，選擇一個可用的逐步案例，然後按照說明操作即可。

![](assets/onboarding.png){width="70%" align="left"}

## 支援的瀏覽器 {#browsers}

Campaign v8 Web 目的是要在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中以最佳方式運作。您可能無法在舊版本或其他瀏覽器上使用某些功能。

## 語言偏好設定 {#language-pref}

Campaign v8 Web 目前提供以下語言版本：

<table>
<tr>
<td>
<p>英文 (US) - EN-US</p>
<p>法文 - FR</p>
<p>德文 - DE</p>
<p>義大利文 - IT</p>
</td>
<td>
<p>西班牙文 - ES</p>
<p>葡萄牙文 (巴西) - PTBR</p>
<p>日文 - JP</p>
</td>
<td>
<p>韓文 - KR</p>
<p>簡體中文 - CHS</p>
<p>繁體中文 - CHT</p>
</td>
</tr>
</table>

您的預設介面語言由使用者設定檔中指定的偏好語言決定。

若要變更您的語言：

1. 按一下右上角您的設定檔圖示，然後選取「**偏好設定**」。

   ![](assets/preferences.png){width="70%" align="left"}

1. 然後，按一下您電子郵件地址下顯示的語言。

   ![](assets/preferences2.png)

1. 選取您偏好的語言，然後按一下「**儲存**」。您可以選取第二語言，以防您使用的元件沒有您第一語言的版本。

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="SMS 報告摘要"
>abstract="探索簡訊傳遞的報告量度。"

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="發佈報告摘要"
>abstract="探索推送傳遞的報告量度。"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推播通知範本"
>abstract="待定"


>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="規則產生器進階屬性"
>abstract="使用進階屬性來定義規則。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="傳送的量度"
>abstract="傳遞的電子郵件數目。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="錯誤量度"
>abstract="具有錯誤狀態的電子郵件數目。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="發佈 Android 內容"
>abstract="定義推播Android內容。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="發佈 iOS 內容"
>abstract="定義推播iOS內容。"

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="應用程式訂閱者"
>abstract="將應用程式訂閱者新增至主要目標，以預覽和測試訊息。 "

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="測試母體"
>abstract="選取測試母體模式。"

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="預覽模式"
>abstract="將測試母體包含至主要目標以預覽和測試訊息。"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="擴充資料"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="個人化"
>abstract="待定"


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="報告傳送"
>abstract="請參閱傳送指標，以取得行銷活動報告。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="報告追蹤"
>abstract="請參閱行銷活動報告的追蹤指標。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="報告概觀"
>abstract="傳遞的關鍵量度。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="報告目標統計資料"
>abstract="此區段會根據對象顯示特定量度。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="傳遞的彙總報告"
>abstract="至少選取兩個傳遞來顯示彙總資料報表。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="重複資料刪除 - 重複欄位"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="重複資料刪除 - 重複設定"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="重複資料刪除 - 重複補充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="維度補充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要權限"
>abstract="您的管理員必須先授予您許可權，您才能建立區段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要權限"
>abstract="您的管理員必須先授予您許可權，您才能建立區段。"

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="屬性選擇器進階欄位"
>abstract="使用進階欄位設定欄。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="規則產生器進階欄位"
>abstract="使用進階欄位設定欄。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="推播傳遞屬性"
>abstract="管理推送傳遞屬性。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新增隔離量度"
>abstract="新增隔離量度。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="簡訊範本選擇"
>abstract="選取預先定義的範本以開始您的SMS傳送。"
