---
audience: end-user
product: campaign
title: 使用內容範本
description: 瞭解如何建立範本以重複使用Adobe Campaign電子郵件中的內容
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="有限可用性"
source-git-commit: 0d9d61e8561d21bca00cb5c274884624119eaa53
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 15%

---

# 使用內容範本 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="定義您自己的內容"
>abstract="從頭開始建立獨立的自訂範本，使您的內容可在多個電子郵件中重複使用。"

為了加快和改進設計流程，您可以建立獨立的範本，以輕鬆地重複使用中的自訂內容 [!DNL Adobe Campaign].

此功能可讓內容導向的使用者使用獨立的範本，以便行銷使用者可以重複使用並在其自己的電子郵件行銷活動中調整它們。

>[!NOTE]
>
>目前僅適用 **電子郵件** 支援內容範本。

## 存取並管理範本 {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="編輯您的範本內容"
>abstract="按一下「**編輯內容**」按鈕可使用電子郵件設計工具更新您的內容。"

若要存取內容範本清單，請選取 **[!UICONTROL 內容管理]** > **[!UICONTROL 內容範本]** 從左側功能表。

![](assets/content-template-list.png)

所有已建立的範本 — 來自使用 [另存為範本](#save-as-template) 選項，選自 **[!UICONTROL 內容範本]** 功能表 — 顯示。

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

您可以篩選特定 [資料夾](../get-started/permissions.md#folders) 使用下拉式清單，或使用新增規則 [查詢模型工具](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

若要編輯範本內容，請從清單中按一下所需的專案。 您可以：

* 編輯其屬性。

* 按一下 **[!UICONTROL 編輯內容]** 按鈕以使用更新您的內容 [電子郵件設計工具](get-started-email-designer.md).

![](assets/content-template-edition.png)

若要刪除範本，請選取範本中 **[!UICONTROL 更多動作]** 功能表。

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>刪除範本時，使用此範本建立的傳遞不會受到影響。

## 建立內容範本 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="內容範本設計"
>abstract="內容範本設計"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="內容範本選擇"
>abstract="內容範本選擇"

建立內容範本的方式有兩種：

* 使用左側邊欄，從頭開始建立內容範本 **[!UICONTROL 內容範本]** 功能表。 [了解做法](#create-template-from-scratch)

* 設計電子郵件時，請將電子郵件內容儲存為範本。 [了解做法](#save-as-template)

儲存後，無論是從草稿還是從先前的電子郵件建立，您現在都可以在建立任何範本時使用此範本 [電子郵件](../email/create-email.md) 範圍 [!DNL Adobe Campaign]. [了解做法](use-email-templates.md)

>[!NOTE]
>
>* 對內容範本所做的變更不會傳播至電子郵件。
>
>* 同樣地，在電子郵件中使用範本時，您對電子郵件內容所做的任何編輯都不會影響先前使用的內容範本。

### 從頭開始建立範本 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="定義您的範本屬性"
>abstract="從頭開始建立範本時，請定義其屬性以便在需要時輕鬆擷取。"

若要從頭開始建立內容範本，請遵循下列步驟。

1. 透過存取內容範本清單 **[!UICONTROL 內容管理]** > **[!UICONTROL 內容範本]** 左側功能表。

1. 選取 **[!UICONTROL 建立範本]**.

   ![](assets/content-template-create.png)

1. 填寫範本詳細資訊。 您可以選取要儲存範本的資料夾。 依預設，內容範本儲存在Adobe Campaign階層的專用資料夾中： **[!UICONTROL 瀏覽器]** > **[!UICONTROL 資源]** > **[!UICONTROL 範本]** > **[!UICONTROL 內容範本]**. [瞭解如何建立資料夾](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >目前僅限 **電子郵件** 頻道和 **HTML** 型別受到支援。

1. 按一下 **[!UICONTROL 建立]** 並從不同選項中選擇要如何設計範本：

   * [從草稿開始設計您的電子郵件](create-email-content.md) 透過電子郵件設計工具的介面。

   * [程式碼或複製貼上原始HTML](code-content.md) 直接放入電子郵件設計工具。

   * [匯入現有的HTML內容](existing-content.md) 檔案或.zip資料夾中的檔案。

   * 使用內建或自訂範本清單中的現有內容。 在電子郵件中使用內容範本的步驟已說明，請參閱 [本節](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. 此 [電子郵件設計工具](get-started-email-designer.md) 顯示。 視需要編輯您的內容，就像根據您選取的選項對任何電子郵件所做的那樣。

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. 範本準備就緒後，按一下 **[!UICONTROL 儲存]**.

   如有需要，請按一下範本名稱旁的箭頭，以返回 **[!UICONTROL 詳細資料]** 畫面並編輯您的範本。

   ![](assets/content-template-save-back.png)

範本會儲存至Adobe Campaign階層的預設資料夾(**[!UICONTROL 瀏覽器]** > **[!UICONTROL 資源]** > **[!UICONTROL 範本]** > **[!UICONTROL 內容範本]**)。 [進一步瞭解資料夾](../get-started/permissions.md#folders)

它也會顯示在 **[!UICONTROL 內容範本]** 清單。 [了解更多](#access-manage-templates)

您現在可以使用此範本建立新內容：此範本位於 **[!UICONTROL 已儲存的範本]** 電子郵件設計工具的索引標籤。 [了解做法](use-email-templates.md)

### 將電子郵件內容另存為範本 {#save-as-template}

一旦您 [設計電子郵件](create-email-content.md)，您可以將此內容儲存為範本以供日後重複使用。 儲存的範本可供 Adobe Campaign 環境的所有使用者使用。

若要將電子郵件內容另存為範本，請依照以下步驟操作：

1. 在電子郵件設計工具中，按一下 **[!UICONTROL 更多]** 按鈕。

1. 選取 **[!UICONTROL 另存為內容範本]** （從下拉式功能表）。

   ![](assets/email_designer-save-template.png)

1. 輸入此範本的名稱，然後儲存。

   ![](assets/email_designer-template-name.png)

範本會儲存至Adobe Campaign階層的預設資料夾(**[!UICONTROL 瀏覽器]** > **[!UICONTROL 資源]** > **[!UICONTROL 範本]** > **[!UICONTROL 內容範本]**)。 [進一步瞭解資料夾](../get-started/permissions.md#folders)

它也會顯示在 **[!UICONTROL 內容範本]** 清單。 它會變成獨立的內容範本，可以像該清單上的任何其他專案一樣加以存取、編輯及刪除。 [了解更多](#access-manage-templates)

您現在可以使用此範本建立新內容：此範本位於 **[!UICONTROL 已儲存的範本]** 電子郵件設計工具的索引標籤。 [了解做法](use-email-templates.md)

![](assets/email_designer-saved-template.png)

>[!NOTE]
>
>對該新範本所做的任何變更都不會傳播到該範本來自的電子郵件。 同樣地，在該電子郵件中編輯原始內容時，不會修改新範本。

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->



