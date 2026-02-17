---
title: 關於綱要
description: 瞭解如何使用結構描述。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# 關於綱要 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="結構描述"
>abstract="Adobe Campaign使用XML型結構描述來定義應用程式中資料的實體和邏輯結構。 在此畫面中，您可以直接從Web使用者介面檢視所有現有方案、存取方案詳細資料、設定自訂表單，以及建立或擴充方案。"

**[!DNL Adobe Campaign]** 使用 XML 型結構描述來定義應用程式內資料的物理和邏輯結構。架構是連結至資料庫表格的XML檔案，其定義：

* SQL表格結構，包括表格名稱、欄位和關係。
* XML資料結構，包括元素、屬性、階層、型別、預設值和標籤。

結構描述在以下方面發揮著關鍵作用：

* 將應用程式資料對應至資料庫表格。
* 定義資料物件之間的關係。
* 指定每個欄位的結構和屬性。

Adobe Campaign中的每個實體都有專屬的結構描述，以確保資料一致性和組織。

結構介面可讓您：

* [存取和自訂結構描述](schemas-browse-access.md) — 檢視可用的結構描述、探索其詳細資訊並自訂熒幕顯示
* [設定清單欄](schemas-list-columns.md) — 設定清單檢視中預設顯示的欄。
* [編輯自訂欄位](schemas-custom-fields.md) — 設定哪些自訂欄位會顯示在詳細畫面中，並將它們組織成區段。
* [新增集合清單](schemas-collection-lists.md) — 新增集合清單，以在設定檔畫面中顯示相關資料。
* [建立和管理結構描述](schemas-create-publish.md#create-schemas) — 建立新結構描述並擴充現有結構描述
* [發佈並同步結構描述](schemas-create-publish.md#publish) — 同步結構描述變更與資料庫結構。
* [使用自訂表單](schemas-custom-forms.md) — 使用資料輸入表單建立、編輯和管理自訂結構描述中的記錄。

>[!NOTE]
>
>您需要有管理員許可權才能管理結構描述。

有關綱要的詳細資訊，請參閱[Campaign主控台檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}。
