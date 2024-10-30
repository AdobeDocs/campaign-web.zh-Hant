---
audience: end-user
product: campaign
title: 使用內容範本
description: 瞭解如何建立範本以重複使用Adobe Campaign電子郵件中的內容
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 0b85b5a4b6eff4fdb9835a0d1ccb5d0a86c103a0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 17%

---

# 使用內容範本 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="內容範本"
>abstract="為了加快和改進設計流程，您可以建立獨立電子郵件範本，以輕鬆地在 Adobe Campaign 中重複使用自訂內容。這些內容範本可以根據內建或自訂範本從頭開始設計、從現有內容建立，或在內容範本編輯器中匯入。"

為了加速並改善設計流程，您可以建立獨立的範本，以輕鬆地在[!DNL Adobe Campaign]中重複使用自訂內容。 這些內容範本可以根據內建或自訂範本從頭開始設計、從現有內容建立，或在內容範本編輯器中匯入。

此功能可讓內容導向的使用者使用獨立的範本，以便行銷使用者可以重複使用並在其自己的電子郵件行銷活動中調整它們。

>[!NOTE]
>
>目前僅支援&#x200B;**電子郵件**&#x200B;內容範本。

## Access 內容範本 {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="編輯您的範本內容"
>abstract="按一下「**編輯內容**」按鈕可使用電子郵件設計工具更新您的內容。"

若要存取內容範本清單，請從左側邊欄瀏覽至&#x200B;**[!UICONTROL 內容管理]** > **[!UICONTROL 內容範本]**&#x200B;功能表。

![](assets/content-template-list.png){zoomable="yes"}

此儀表板會將所有可用的內容範本顯示為清單。 您可以使用下拉式清單篩選特定[資料夾](../get-started/permissions.md#folders)，或使用[查詢模型工具](../query/query-modeler-overview.md)新增規則。

![](assets/content-template-list-filters.png){zoomable="yes"}

您可以從清單中編輯、複製或刪除現有的內容範本。 使用上半區段的按鈕來建立內容範本。

### 唯讀模式下的內容範本 {#template-readonly}

存取許可權可套用至內容範本。

如果您沒有特定內容範本的編輯許可權，內容範本會以&#x200B;**唯讀模式**&#x200B;顯示。 在此情況下，**[!UICONTROL 編輯內容]**&#x200B;按鈕會取代為&#x200B;**[!UICONTROL 檢視內容]**&#x200B;按鈕，讓您檢視範本而不做任何變更。

![](assets/template-readonly.png){zoomable="yes"}

如下所示，所有功能圖示都會停用，限制僅供檢視互動。

![](assets/template-readonly-view.png){zoomable="yes"}

## 建立內容範本 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="內容範本設計"
>abstract="設計您的電子郵件內容範本。"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="內容範本選擇"
>abstract="選取您的電子郵件內容範本。"

內容範本可透過[將現有電子郵件儲存為範本](#save-as-template)，或從電子郵件範本清單中，透過&#x200B;**建立內容範本**&#x200B;按鈕[建立，詳情如下](#create-template-from-scratch)。

儲存後，您現在可以在[!DNL Adobe Campaign]內建立任何[電子郵件](../email/create-email.md)時使用此範本。 [了解做法](use-email-templates.md)

>[!NOTE]
>
>* 對內容範本所做的變更不會傳播至電子郵件。
>
>* 同樣地，在電子郵件中使用範本時，您對電子郵件內容所做的任何編輯都不會影響先前使用的內容範本。

### 建立新的內容範本 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="定義您的範本屬性"
>abstract="定義您的電子郵件內容範本屬性，以便在需要時輕鬆擷取。"

若要從內容範本控制面板建立新的內容範本，請執行下列步驟：

1. 從&#x200B;**[!UICONTROL 內容管理]** > **[!UICONTROL 內容範本]**&#x200B;左側邊欄瀏覽至內容範本清單。

1. 選取&#x200B;**[!UICONTROL 建立範本]**。

   ![](assets/content-template-create.png){zoomable="yes"}

1. 輸入範本標籤和屬性。 您可以選取要儲存範本的資料夾。 依預設，內容範本儲存在Adobe Campaign階層的專用資料夾中： **[!UICONTROL 檔案總管]** > **[!UICONTROL 資源]** > **[!UICONTROL 範本]** > **[!UICONTROL 內容範本]**。 在[此頁面](../get-started/permissions.md#folders)中進一步瞭解資料夾

   ![](assets/content-template-details.png){zoomable="yes"}

1. 按一下「建立&#x200B;**[!UICONTROL 」]**，然後從不同的選項中選擇要如何設計範本：

   * [透過Designer的電子郵件介面從草稿開始設計您的內容](create-email-content.md)。

   * [直接將原始HTML](code-content.md)編碼或複製貼上到Designer電子郵件中。

   * [從檔案或.zip資料夾匯入現有的HTML內容](existing-content.md)。

   * 使用內建或自訂範本清單中的現有內容。 在[本節](use-email-templates.md)中說明在電子郵件中使用內容範本的步驟。

   ![](assets/email_designer-templates.png){zoomable="yes"}

1. Designer電子郵件隨即顯示。 視需要編輯您的內容，就像根據您選取的選項對任何電子郵件所做的那樣。 在[本節](get-started-email-designer.md)中瞭解如何使用電子郵件Designer。

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. 範本準備就緒後，請按一下[儲存]。****

   如有需要，請按一下範本名稱旁的箭頭，返回&#x200B;**[!UICONTROL 詳細資料]**&#x200B;畫面並編輯您的範本。

   ![](assets/content-template-save-back.png){zoomable="yes"}

範本可在&#x200B;**[!UICONTROL 內容範本]**&#x200B;清單中使用。 [了解更多](#access-templates)

您現在可以使用此範本建立新內容：可在電子郵件Designer的&#x200B;**[!UICONTROL 已儲存範本]**&#x200B;索引標籤中找到它。 [了解做法](use-email-templates.md)

### 將電子郵件內容另存為範本 {#save-as-template}

當您[設計電子郵件](create-email-content.md)後，您可以將此內容儲存為範本，以供日後重複使用。 儲存的範本可供 Adobe Campaign 環境的所有使用者使用。

若要將電子郵件內容另存為範本，請依照以下步驟操作：

1. 在電子郵件設計工具中，按一下畫面右上方的&#x200B;**[!UICONTROL 更多]**&#x200B;按鈕。

1. 從下拉式功能表中選取&#x200B;**[!UICONTROL 另存為內容範本]**。

   ![](assets/email_designer-save-template.png){zoomable="yes"}

1. 輸入此範本的名稱，然後儲存。

   ![](assets/email_designer-template-name.png){zoomable="yes"}

範本已儲存並顯示在&#x200B;**[!UICONTROL 內容範本]**&#x200B;清單中。 它會變成獨立的內容範本，可以像該清單上的任何其他專案一樣加以存取、編輯及刪除。 [了解更多](#access-manage-templates)

您現在可以使用此範本建立新內容：可在電子郵件Designer的&#x200B;**[!UICONTROL 已儲存範本]**&#x200B;索引標籤中找到它。 [了解做法](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable="yes"}


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


## 修改內容範本 {#modify-delete}

若要更新現有的內容範本，請遵循下列步驟：

1. 從內容範本清單中，按一下要修改的範本標籤以進行編輯。

1. 按一下&#x200B;**[!UICONTROL 編輯內容]**&#x200B;按鈕，使用[電子郵件Designer](get-started-email-designer.md)更新您的內容。

![](assets/content-template-edition.png){zoomable="yes"}

>[!NOTE]
>
>使用此內容範本時，對內容範本所做的變更不會傳播至電子郵件。

## 刪除內容範本 {#content-delete}

刪除內容範本有兩個方法：

* 從內容範本清單中，按一下省略符號按鈕，然後選取&#x200B;**刪除**

  ![從儀表板刪除內容範本](assets/content-template-list-delete.png)

* 從內容範本本身，按一下&#x200B;**更多**&#x200B;按鈕，然後選取&#x200B;**刪除**


>[!NOTE]
>
>刪除內容範本不會影響使用此範本建立的傳送。


## 複製內容範本 {#content-duplicate}

複製內容範本有兩個方法：

* 從內容範本清單中，按一下省略符號按鈕，然後選取&#x200B;**複製**

* 從內容範本本身，按一下&#x200B;**更多**&#x200B;按鈕，然後選取&#x200B;**複製**

在這兩種情況下，請確認複製以建立新的內容範本。 新內容範本的標籤是&#x200B;**`<label of the initial campaign`**&#x200B;的復本。 瀏覽至範本設定以更新此標籤。

