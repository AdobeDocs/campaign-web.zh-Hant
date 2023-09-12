---
audience: end-user
title: Campaign網站中的許可權管理
description: 進一步瞭解Campaign網頁v8中的許可權
badge: label="Beta"
source-git-commit: 3cd540af6ccccdecc4d41983d4d11ffb1ea72c43
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 1%

---


# 存取權與權限 {#access-and-permissions}


>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="需要權限"
>abstract="您的管理員必須先授予您許可權，您才能建立此物件。"



存取控制可限制存取主要清單中的物件和資料，例如傳遞、收件者或工作流程。 這些限制也會套用在Explorer導覽樹狀結構中。 此外，您需要許可權才能從使用者介面建立、刪除、複製及編輯物件。

存取控制是在使用者端主控台中進行管理。 Campaign Web中的所有許可權都會與Campaign使用者端主控台許可權同步。 只有Campaign管理員可以定義及修改使用者許可權。 進一步瞭解中的使用者許可權 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}.

瀏覽Campaign Web使用者介面時，您可以存取資料、物件和功能，具體取決於您的許可權。 例如，如果您沒有資料夾的存取許可權，您將無法看到它。 您的許可權也會影響物件和資料管理。 沒有特定資料夾的寫入許可權，您無法在該資料夾中建立傳送，即使您可以在使用者介面中看到該傳送。

## 檢視許可權 {#view-permissions}

從 **瀏覽器**，您可以瀏覽每個檔案夾的許可權。 這些許可權是在使用者端主控台中設定，用於組織和控制Campaign資料的存取。


若要檢視檔案夾的許可權，請執行下列步驟：

1. 從 **瀏覽器** 在左側導覽選單中，選取資料夾。
1. 按一下右上角的三個點，然後選取 **檔案夾許可權**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. 在畫面中檢視詳細資訊，如下所示：

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   群組或運運算元可擁有對儲存在所選資料夾中之資料的讀取、寫入及/或刪除許可權。

   如果 **傳播** 選項已啟用，針對檔案夾定義的所有許可權都會套用至其所有子檔案夾。 每個子檔案夾都可以多載這些許可權。

   如果 **系統資料夾** 選項已啟用，允許所有運運算元存取，無論其許可權為何。

進一步瞭解中的檔案夾許可權 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## 使用資料夾 {#folders}

您可以建立、重新命名、重新排序和行動資料夾來組織您的元件和資料。 您也可以從相同功能表刪除資料夾。

>[!CAUTION]
>
>刪除資料夾時，也會刪除儲存在該資料夾中的所有資料。

若要建立資料夾，請執行下列步驟：

1. 從 **瀏覽器** 在左側導覽選單中，選取資料夾。
1. 按一下右上角的三個點，然後選擇 **建立新的子資料夾**.
1. 輸入資料夾名稱並儲存。

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   資料夾會新增為目前資料夾的子資料夾。 瀏覽到該新資料夾以直接在該資料夾中建立元件。 您也可以從任何資料夾中建立元件，然後將其儲存在該新資料夾的 **其他選項** 屬性的區段，如下所示：

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

