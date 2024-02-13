---
title: 在Campaign中建立測試設定檔
description: 瞭解如何在Adobe Campaign中建立和管理測試設定檔
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 13%

---

# 建立和管理測試設定檔 {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="建立測試設定檔"
>abstract="測試設定檔為種子地址。他們是資料庫中的額外收件者，用於找出與定義的目標標準不相符的虛構設定檔。"

測試設定檔為種子地址。他們是資料庫中用於鎖定不符合已定義目標條件之虛擬設定檔的其他收件者。 附註可讓您在傳送傳遞前，透過傳送校樣來預覽及測試個人化和轉譯。

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

將測試訊息傳送至種子地址的步驟詳見 [本節](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>測試設定檔會自動從下列傳送統計資料的報告排除： **[!UICONTROL 點按次數]**， **[!UICONTROL 開啟次數]**， **[!UICONTROL 取消訂閱]**. [進一步瞭解報告]

## 存取及管理測試設定檔 {#access-test-profiles}

若要存取測試設定檔清單，請選取 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 從左側功能表，然後按一下 **[!UICONTROL 測試設定檔]** 標籤。

![](assets/test-profile-list.png){zoomable=&quot;yes&quot;}

* 您可以篩選特定 [資料夾](../get-started/permissions.md#folders) 使用下拉式清單，或使用新增規則 [查詢模型工具](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png){zoomable=&quot;yes&quot;}

* 您可以複製任何測試設定檔，並視需要更新。 編輯測試設定檔的步驟與以下相同： [建立測試設定檔](#create-test-profile).

* 若要刪除測試設定檔，請從 **[!UICONTROL 更多動作]** 功能表。

  ![](assets/test-profile-list-delete.png){zoomable=&quot;yes&quot;}

* 若要編輯測試設定檔，請從清單中按一下所需的專案。 編輯測試設定檔的步驟與以下相同： [建立測試設定檔](#create-test-profile).

您也可以透過存取測試設定檔 **[!UICONTROL 瀏覽器]** 檢視，從 **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子地址]** 節點。

您可以從中瀏覽、建立和管理檔案夾或子檔案夾，以及檢查關聯的許可權。 [瞭解如何建立資料夾](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png){zoomable=&quot;yes&quot;}

從 **[!UICONTROL 瀏覽器]** 檢視您也可以篩選、刪除、編輯和 [建立](#create-test-profile) 測試設定檔。

## 建立測試設定檔 {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="測試設定檔的附加資料"
>abstract="輸入個人化資料，此個人化資料用於資料管理工作流程中建立的傳遞，並且您要為其指派特定值。"

若要建立測試設定檔，請遵循下列步驟。

1. 瀏覽至 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 並選取 **[!UICONTROL 測試設定檔]** 標籤。

1. 按一下 **[!UICONTROL 建立測試設定檔]** 按鈕。

   ![](assets/test-profile-create.png){zoomable=&quot;yes&quot;}

1. 視需要填寫測試設定檔的詳細資料。 <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >此 **[!UICONTROL 標籤]** 欄位會自動填入您定義的名字和姓氏。

1. 依預設，測試設定檔儲存在 **[!UICONTROL 種子地址]** 資料夾。 您可以瀏覽至所需的位置來變更它。 [瞭解如何使用資料夾](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. 在 **[!UICONTROL 連絡資訊]** 區段，輸入電子郵件地址及其他相關資料。 電子郵件地址會顯示在測試設定檔標籤後的方括弧之間。

   ![](assets/test-profile-address.png){zoomable=&quot;yes&quot;}

1. 如果您選取 **[!UICONTROL 不再聯絡（透過任何管道）]** 核取方塊，測試設定檔位於封鎖清單上。 任何頻道（電子郵件、簡訊等）不再以這類收件者為目標。

1. 在 **[!UICONTROL 其他資料]** 標籤，輸入在資料管理工作流程中建立且您想要指派特定值的傳遞所使用的個人化資料。 [進一步瞭解工作流程](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png){zoomable=&quot;yes&quot;}

   請確定已在中定義其他目標資料，且別名開頭為&#39;@&#39;。 **[!UICONTROL 擴充]** 工作流程活動。 否則，您就無法在傳遞活動中正確搭配種子地址使用。 [進一步瞭解擴充活動](../workflows/activities/enrichment.md)

1. 按一下 **[!UICONTROL 儲存]** 按鈕。

您剛建立的測試設定檔現已準備就緒，可用來傳送測試。 [了解更多](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->
