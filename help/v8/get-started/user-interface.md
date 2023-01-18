---
audience: end-user
title: 探索介面
description: Campaign v8 Web使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: b203d1e2adb1b41cdc4adf398934707f6093b317
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 1%

---

# 探索介面 {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="探索介面"
>abstract="新的Campaign v8 Web介面提供整合、直覺且一致的使用者體驗。"

新的Campaign v8網頁介面提供現代且直覺的使用者體驗，以簡化行銷活動的設計和傳遞。 此新介面已與Adobe Experience Platform整合。

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>本檔案會經常更新，以反映產品使用者介面的最新變更。 不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左側導覽功能表

瀏覽左側的連結，以存取Campaign v8 Web功能。 有幾個連結顯示可排序和篩選的對象清單。 您也可以設定欄以顯示您需要的所有資訊。 看這個 [節](#list-screens). 除電子郵件傳送清單外，所有清單畫面均為唯讀。 按一下任何清單項目即無法在Alpha中使用版本/檢視功能。 所有清單都可在未來版本中編輯。 左側導覽功能表中顯示的項目取決於您的使用者權限。

![](assets/home.png)

### 首頁

此畫麵包含快速存取主要Campaign v8 Web功能的關鍵連結和資源。 此 **收件者** 清單提供最近建立和修改的傳送的捷徑。 此清單顯示其建立和修改日期與狀態。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

從首頁的下半部存取Campaign v8網路金鑰說明頁面。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### 探索工具

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="此 **瀏覽器** 菜單顯示與客戶端控制台中的資料夾層次結構相同的資料夾層次結構。 瀏覽您所有的Campaign v8元件、資料夾和結構。 除電子郵件傳送清單外，所有清單畫面均為唯讀。"

此 **瀏覽器** 菜單顯示與客戶端控制台中的資料夾層次結構相同的資料夾層次結構。 瀏覽您所有的Campaign v8元件、資料夾和結構。 除電子郵件傳送清單外，所有清單畫面均為唯讀。

瀏覽器中顯示的項目取決於您的使用者權限。

如同在任何清單畫面中，您可以設定欄以個人化顯示，以檢視您需要的所有資訊。 看這個 [節](#list-screens).

如需Campaign總管的詳細資訊，請參閱 [檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="行銷活動"
>abstract="這是您的行銷活動清單。 您可以檢視有用的資訊，例如其開始/結束/最後修改日期，以及其狀態。 您可以依狀態或開始/結束日期篩選清單。 也提供行銷活動範本。 這些清單為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="傳遞"
>abstract="瀏覽傳遞清單。 您可以檢視其狀態、上次修改日期以及關鍵KPI。 您可以依州、聯絡人日期或管道篩選清單。 按一下電子郵件傳送以開啟其控制面板。 其他項目為唯讀。 也提供傳遞範本。"

* **行銷活動**  — 此為促銷活動清單。 依預設，您可以檢視其開始/結束/最後修改日期及其狀態。 您可以依狀態或開始/結束日期篩選清單。 也提供行銷活動範本。 這些清單為唯讀清單。

* **傳遞**  — 瀏覽傳遞清單。 依預設，您可以檢視其狀態、上次修改日期以及關鍵KPI。 您可以依州、聯絡人日期或管道篩選清單。 按一下電子郵件傳送以開啟其控制面板，以取得傳送詳細資料的概觀。 其他通道上的傳送為唯讀。 傳遞範本也以唯讀模式提供。 您可以使用用戶端主控台來編輯。 看這個 [檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   使用 **更多動作** 按鈕來刪除或複製傳送。

   ![](assets/more-actions.png){width="70%" align="left"}

### 客戶管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="收件者"
>abstract="存取收件者資料庫。 您可以檢視實用資訊，例如其電子郵件地址、名字和姓氏。 此清單為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="對象"
>abstract="這是您的對象清單。 您可以檢視其類型、來源、建立/上次修改日期和標籤。 您可以依來源篩選清單。 此清單為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="訂閱清單"
>abstract="瀏覽訂閱清單。 您可以檢視其類型、模式和標籤。 此清單為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="目標定位工作流程"
>abstract="存取Campaign工作流程清單。 您可以檢視其狀態、上次/下次處理日期和環境。 您可以依狀態、上次處理日期和工作流程類型來篩選清單。 也提供工作流程範本。 這些清單為唯讀清單。"

* **收件者**  — 訪問您的收件者資料庫。 依預設，您可以檢視其電子郵件地址、名字和姓氏。 此清單為唯讀清單。
* **對象**  — 此為您的對象清單。 依預設，您可以檢視其類型、來源、建立/上次修改日期和標籤。 您可以依來源篩選清單。 此清單為唯讀清單。
* **訂閱清單**  — 瀏覽訂閱清單。 依預設，您可以檢視其類型、模式和標籤。 此清單為唯讀清單。
* **目標工作流程**  — 存取Campaign工作流程清單。 依預設，您可以檢視其狀態、上次/下次處理日期和環境。 您可以依狀態、上次處理日期和工作流程類型來篩選清單。 也提供工作流程範本。 這些清單為唯讀清單。

### 決策管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="優惠"
>abstract="瀏覽您的互動選件清單。 依預設，您可以檢視其狀態、開始/結束日期和環境。 您可以依狀態和開始/結束日期篩選清單。 也提供優惠方案範本。 這些清單為唯讀清單。"

* **選件**  — 瀏覽您的互動選件清單。 依預設，您可以檢視其狀態、開始/結束日期和環境。 您可以依狀態和開始/結束日期篩選清單。 也提供優惠方案範本。 這些清單為唯讀清單。

## 頂端列

介面的頂端列可讓您：

* 以Alpha測試者的身分分享您的意見
* 在組織和實例之間切換
* 在Adobe Experience Cloud應用程式之間切換
* 存取說明頁面、聯絡支援及分享意見。 您可以從搜尋欄位搜尋說明文章和影片。

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 設定清單畫面 {#list-screens}

例如，左側導覽功能表中的數個連結 **傳遞** 或 **行銷活動**，顯示對象清單。 這些清單畫面是唯讀的，但電子郵件傳送清單除外。

若要更快找到項目，您可以使用搜尋列，或根據內容條件篩選清單。

![](assets/filter.png){width="70%" align="left"}

清單會以欄顯示。 您可以變更欄組態以顯示其他資訊。 若要這麼做，請按一下清單右上角的圖示。 您可以新增或移除欄，並變更其顯示順序。

![](assets/columns.png){width="70%" align="left"}

您可以按一下任何欄標題，以排序清單中的項目。 將顯示一個箭頭（向上或向下），指明清單按該列排序。 對於數值或日期欄，向上箭頭表示清單是以升序排序，而向下箭頭表示降序。 對於字串或英數字元列，值按字母順序列出。

## 內容說明與入門指南

介面中提供內容說明。 可用時，按一下 **?** 圖示來顯示說明資訊和相關檔案連結。

![](assets/context-help.png){width="70%" align="left"}

也提供上線指南，協助您開始使用Campaign v8 Web。 按一下右下角的圖示，選擇任一可用的逐步案例，然後只需依照指示操作即可。

![](assets/onboarding.png){width="70%" align="left"}

## 支援的瀏覽器 {#browsers}

Campaign v8 Web在最新版Google Chrome、Safari和Microsoft Edge中可以最佳化運作。 您在舊版或其他瀏覽器上使用某些功能時可能遇到問題。

## 語言偏好設定 {#language-pref}

使用者介面目前提供下列語言：

* 英語（美國） — EN-US
* 法語 — FR
* 德文 — DE
* 義大利語 — IT
* 西班牙文 — ES
* 葡萄牙語（巴西） — PTBR
* 日文 — JP
* 韓語 — KR
* 簡體中文 — CHS
* 繁體中文 — CHT

您的預設介面語言由使用者設定檔中指定的偏好語言決定。

若要變更您的語言：

* 按一下 **偏好設定** 從你的頭像，在右上角。
   ![](assets/preferences.png)
* 然後按一下您電子郵件地址下方顯示的語言
* 選取您偏好的語言，然後按一下 **儲存**. 您可以選取第二種語言，以備您使用的元件未以第一種語言本地化時使用。
   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->