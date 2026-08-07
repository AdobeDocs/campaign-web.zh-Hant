---
title: 品牌化
description: 瞭解如何設定您的品牌
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 5c9d3db95905f77dddffaf824156c87b9d79013c
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 10%

---

# 設定品牌 {#branding-configure}

技術管理員可以直接從Web UI建立和管理多個品牌。 這可讓您定義構成品牌身分識別的所有元素，包括標誌，甚至電子郵件追蹤設定。

>[!NOTE]
>
>此功能需要您執行個體上的品牌套件。 如果您看不到&#x200B;**品牌**&#x200B;功能表，請聯絡您的Adobe代表。

## 建立或編輯品牌 {#create-edit-brand}

>[!CONTEXTUALHELP]
>id="acw_branding_create"
>title="建立品牌"
>abstract="按一下「**建立品牌**」以定義新的品牌識別。 在「設定」標記中填寫品牌詳細資訊，然後按一下「**建立品牌**」以儲存。 此品牌將可連結至傳遞範本和獨立傳遞。"

若要建立新品牌，請遵循下列步驟：

1. 從左側功能表瀏覽至&#x200B;**[!UICONTROL 管理>品牌]**，或從&#x200B;**[!UICONTROL 總管]**&#x200B;瀏覽至&#x200B;**[!UICONTROL 管理>平台>品牌]**。

1. 按一下清單上方的&#x200B;**[!UICONTROL 建立品牌]**&#x200B;按鈕。

   ![顯示品牌建立的熒幕擷圖](assets/branding-create.png)

1. 填寫不同區段的品牌詳細資訊。 下方[品牌屬性](#brand-attributes)區段中會說明每個欄位。

   ![顯示品牌建立欄位的熒幕擷圖](assets/branding-create2.png)

1. 按一下&#x200B;**[!UICONTROL 建立品牌]**&#x200B;以儲存。 品牌現在可連結至傳遞範本和獨立傳遞。 [瞭解如何指派品牌](branding-assign.md)。

若要編輯現有品牌，請從清單中選取該品牌、更新欄位並儲存變更。

## 品牌屬性 {#brand-attributes}

**[!UICONTROL 品牌]**&#x200B;已設定為橫跨四個區段： **[!UICONTROL 身分]**、**[!UICONTROL 品牌設定]**、**[!UICONTROL 電子郵件標頭引數]**&#x200B;以及&#x200B;**[!UICONTROL URL追蹤引數]**。

### 身分識別 {#identity}

**[!UICONTROL 身分]**&#x200B;區段可讓您定義並個人化您的品牌。

![熒幕擷圖顯示建立品牌時的「身分」標籤](assets/branding-create3.png)

本章節包含以下欄位：

* **[!UICONTROL 品牌名稱]**：您的品牌名稱。 此欄位為必填項。
* **[!UICONTROL 標籤]**：介面中可見的標籤。
* **[!UICONTROL ID]**：自動產生內部識別碼。 您可以加以變更。 只允許使用字母、數字和底線。 特殊字元會替換為底線。
* **[!UICONTROL 標誌URL]**：品牌標誌影像的URL。
* **[!UICONTROL 網站URL]**&#x200B;和&#x200B;**[!UICONTROL 網站標籤]**：與品牌關聯的網站URL和標籤。


### 品牌設定 {#brand-configs}

在&#x200B;**[!UICONTROL 品牌設定]**&#x200B;區段中，您定義用於追蹤和登陸頁面存取的子網域和URL通訊協定。

![顯示「品牌設定」索引標籤的熒幕擷圖](assets/branding-create4.png)

本章節包含以下欄位：

* **[!UICONTROL 品牌子網域]**：此品牌專屬的子網域URL已要求從Adobe委派。
* **[!UICONTROL 追蹤URL通訊協定]**、**[!UICONTROL 映象頁面URL通訊協定]**&#x200B;和&#x200B;**[!UICONTROL 應用程式URL通訊協定]**：用於每個URL型別的通訊協定(例如，**安全(https)**)。

>[!NOTE]
>
>追蹤、映象和應用程式伺服器的設定會儲存在與路由相關的個別外部帳戶中。 這些設定會在布建期間套用，且不應加以修改。 若要顯示URL，請從您的外部帳戶存取&#x200B;**[!UICONTROL 品牌首碼]**&#x200B;索引標籤。

### 電子郵件標頭參數 {#header-param}

**[!UICONTROL 電子郵件標頭引數]**&#x200B;可讓您個人化收件者在行銷活動標頭區段中看到的內容。

![熒幕擷圖顯示含有電子郵件標頭欄位的[標頭引數]索引標籤](assets/branding-create5.png)

本章節包含以下欄位：

* **[!UICONTROL 寄件者（電子郵件地址）]**：品牌的電子郵件地址。
* **[!UICONTROL 寄件者（名稱）]**：品牌名稱。
* **[!UICONTROL 回覆（電子郵件地址）]**：客戶可以回覆的電子郵件地址。
* **[!UICONTROL 回覆（名稱）]**：回覆的顯示名稱。
* **[!UICONTROL 錯誤（電子郵件地址）]**：發生錯誤時所使用的電子郵件地址。

<!--
>[!IMPORTANT]
>
>After having updated the header parameters of the emails, if the name and email address of the sender have not changed in the email created from the template, check the template's advanced settings.
-->

### URL 追蹤參數 {#tracking-param}

在&#x200B;**[!UICONTROL URL追蹤引數]**&#x200B;區段中，您可以定義其他引數，以便與Adobe Analytics和Google Analytics等網站分析工具整合，藉此增強URL追蹤。

![在[標頭引數]索引標籤中顯示URL追蹤引數的熒幕擷圖](assets/branding-create6.png)

本章節包含以下欄位：

* **[!UICONTROL 其他URL引數]**：將引數新增為機碼值組及其適用性條件。 每個引數名稱必須是唯一的且非空白，而且每個引數值都必須非空白。 適用性條件可以為空白，但這些值都不能包含JST標籤。

* **[!UICONTROL 網域名稱允許清單]**：新增網域名稱或規則運算式，以符合將附加追蹤引數的URL。

**範例：**&#x200B;當為該網域設定其他引數`age=21`和`deliveryName=DM101`時，類似`https://www.luma.com`的追蹤URL將變成`https://www.luma.com/?age=21&deliveryName=DM101`。

## 設定異動訊息的品牌 {#branding-transactional-config}

>[!IMPORTANT]
>
>本節僅適用於異動訊息（訊息中心）。
>
>雖然Campaign Web UI提供交易功能，但必須在Campaign v8使用者端主控台（控制執行個體）中執行下列步驟。

如果您正在使用交易式訊息（訊息中心）與品牌，則需要額外設定。

### 即時執行個體的追蹤公式

在即時(RT)控制執行個體上啟用品牌化時，會使用特定的追蹤選項來管理追蹤公式。 這些公式是在RT Control執行個體上集中設定，而不是在每個RT Execution執行個體上個別設定。

下列選項會定義RT傳送使用的追蹤公式：

* **`NmsTracking_RT_ClickFormula`**：指定在RT執行個體上用於點選追蹤的公式

* **`NmsTracking_RT_OpenFormula`**：指定用於在RT執行個體上開啟追蹤的公式

如果您的實作需要交易式訊息的自訂追蹤公式，請使用下列選項：

* **`Branding_RT_ListXtkOptions_toPublish`**：在這裡列出自訂公式的XTK選項名稱（以逗號分隔）。 這可確保RT傳送可套用自訂追蹤公式。
