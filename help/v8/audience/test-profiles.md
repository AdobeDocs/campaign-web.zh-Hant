---
title: 在Campaign中建立測試設定檔
description: 瞭解如何在Adobe Campaign中建立和管理測試設定檔
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="有限可用性"
source-git-commit: 59094528cb3683dba7264e6b63b5166a0a91f8ed
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 3%

---

# 建立和管理測試設定檔 {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="建立測試設定檔"
>abstract="測試設定檔會建立為種子地址。 他們是資料庫中用於鎖定不符合已定義目標條件之虛擬設定檔的其他收件者。"

測試設定檔會建立為種子地址。 他們是資料庫中用於鎖定不符合已定義目標條件之虛擬設定檔的其他收件者。 附註可讓您在傳送傳遞前，透過傳送校樣來預覽及測試個人化和轉譯。

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

將測試訊息傳送至種子地址的步驟詳見 [本節](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>測試設定檔會自動從下列傳送統計資料的報告排除： **[!UICONTROL 點按次數]**， **[!UICONTROL 開啟次數]**， **[!UICONTROL 取消訂閱]**.

## 存取及管理測試設定檔 {#access-test-profiles}

若要存取內容範本清單，請選取 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 從左側功能表選取 **[!UICONTROL 測試設定檔]** 標籤。

您可以篩選特定 [資料夾](../get-started/permissions.md#folders) 使用下拉式清單，或使用新增規則 [查詢模型工具](../query/query-modeler-overview.md).

若要編輯測試設定檔，請從清單中按一下所需的專案。

若要刪除測試設定檔，請從 **[!UICONTROL 更多動作]** 功能表。

## 建立測試設定檔 {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="測試個人資料的附加資料"
>abstract="輸入在資料管理工作流程中建立且您想要指派特定值的傳遞所使用的個人化資料。"

若要建立測試設定檔，請遵循下列步驟。

1. 瀏覽至 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]**.

1. 選取 **[!UICONTROL 測試設定檔]** 標籤。

   ![](assets/test-profile-list.png)

1. 按一下 **[!UICONTROL 建立測試設定檔]** 按鈕。

1. 填寫測試設定檔詳細資料。 <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >地址的標籤會自動填入您所定義的名字和姓氏。

1. 依預設，測試設定檔儲存在 **[!UICONTROL 種子地址]** 資料夾。 您可以瀏覽至所需的位置來變更它。 [了解更多](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. 在 **[!UICONTROL 連絡資訊]** 區段，輸入電子郵件地址及其他相關資料。 電子郵件地址會顯示在測試設定檔標籤後的方括弧之間。

   ![](assets/test-profile-address.png)

1. 如果您選取 **[!UICONTROL 不再聯絡（透過任何管道）]** 核取方塊，設定檔位於封鎖清單上。 任何頻道（電子郵件、簡訊等）不再以這類收件者為目標。

1. 在 **[!UICONTROL 其他資料]** 標籤，輸入在資料管理工作流程中建立且您想要指派特定值的傳遞所使用的個人化資料。 [進一步瞭解工作流程](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   請確定已在中定義其他目標資料，且別名開頭為&#39;@&#39;。 **[!UICONTROL 擴充]** 工作流程活動。 否則，您就無法在傳遞活動中正確搭配種子地址使用。 [進一步瞭解擴充活動](../workflows/activities/enrichment.md)

1. 按一下 **[!UICONTROL 儲存]** 按鈕。

您剛建立的測試設定檔現已準備就緒，可用來傳送測試。 [了解更多](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## 管理種子地址資料夾 {#seed-addresses-folders}

種子地址會儲存在Adobe Campaign階層的專用節點中： **[!UICONTROL 瀏覽器]** > **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子地址]**.

若要組織測試設定檔，您可以從「更多動作」下拉式清單中建立子資料夾。 [瞭解如何建立資料夾](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

您也可以從任何 **[!UICONTROL 種子地址]** 資料夾或子資料夾。 請以您從表格中執行操作的方式填入所有詳細資訊。 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 功能表。 [了解更多](#create-test-profile)

若要編輯測試設定檔，請從 **[!UICONTROL 測試設定檔]** 標籤或儲存所在的資料夾中。

