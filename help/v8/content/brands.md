---
audience: end-user
title: 管理品牌
description: 瞭解如何建立和管理您的品牌指引
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 3%

---

# 建立和管理您的品牌 {#brands}

品牌指引是一組完整的規則和標準，可定義品牌的視覺和口頭識別。 這些區段可作為參考，以確保在所有行銷和通訊管道中一致的品牌代表性。

在[!DNL Adobe Campaign Web]中，使用者可以手動輸入及組織品牌資訊，或上傳品牌指引檔案以進行自動資料擷取。

## 存取品牌 {#generative-access}

若要存取&#x200B;**[!UICONTROL 中的]**&#x200B;品牌[!DNL Adobe Campaign Web]功能表，必須指派使用者&#x200B;**[!UICONTROL 管理員（管理員）]**&#x200B;和&#x200B;**[!UICONTROL 品牌套件]**&#x200B;產品設定檔，才能建立和管理品牌。 若為唯讀存取，使用者需要[!UICONTROL AI助理]產品設定檔。 [了解更多](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ 瞭解如何指派品牌相關許可權

1. 在[Admin Console](https://adminconsole.adobe.com/enterprise)首頁中，存取您的行銷活動產品。

   ![Admin Console首頁顯示Campaign產品存取權](assets/brands_admin_1.png)

1. 根據您要授與使用者的許可權層級選取&#x200B;**[!DNL Product profile]**。

   ![Admin Console中的產品設定檔選擇](assets/brands_admin_2.png)

1. 按一下&#x200B;**[!DNL Add users]**&#x200B;以指派選取的產品設定檔。

   ![在Admin Console中新增使用者選項](assets/brands_admin_3.png)

1. 輸入您的使用者名稱、使用者群組或電子郵件地址。

1. 按一下[儲存]以套用變更。****

已指派給此角色的使用者會自動更新其許可權。

+++

## 建立您的品牌 {#create-brand-kit}

若要建立和管理您的品牌指引，請遵循下列步驟。

使用者可以手動輸入詳細資料，或上傳品牌指引檔案以自動擷取資訊：

1. 在&#x200B;**[!UICONTROL 品牌]**&#x200B;功能表中，按一下&#x200B;**[!UICONTROL 建立品牌]**。

   ![具有[建立品牌]選項的[品牌]功能表](assets/brands-1.png)

1. 輸入您品牌的&#x200B;**[!UICONTROL 名稱]**。

1. 拖放或選取您的檔案，以上傳您的品牌指引，並自動擷取相關的品牌資訊。 按一下&#x200B;**[!UICONTROL 建立品牌]**。

   資訊擷取程式現在開始。 請注意，可能需要幾分鐘才能完成。

   ![檔案上傳以供品牌指引擷取](assets/brands-2.png)

1. 系統現在會自動填入您的內容和視覺化建立標準。 瀏覽不同的標籤，視需要調整資訊。 [了解更多](#personalize)

1. 從每個區段或類別的進階功能表中，您可以新增參照以自動擷取相關品牌資訊。

   若要移除現有內容，請使用&#x200B;**[!UICONTROL 清除區段]**&#x200B;或&#x200B;**[!UICONTROL 清除類別]**&#x200B;選項。

   ![](assets/brands-15.png)

1. 設定之後，按一下&#x200B;**[!UICONTROL 儲存]**，然後按一下&#x200B;**[!UICONTROL 發佈]**，讓您的品牌指引可在AI助理中取得。

1. 若要修改您發佈的品牌，請按一下[編輯品牌]。****

   >[!NOTE]
   >
   >這會在編輯模式中建立臨時副本，並在發佈後取代即時版本。

   ![在[品牌]功能表中編輯品牌選項](assets/brands-8.png)

1. 從您的&#x200B;**[!UICONTROL 品牌]**&#x200B;儀表板，按一下![](assets/do-not-localize/Smock_More_18_N.svg)圖示以開啟進階功能表：

   * 檢視品牌
   * 編輯
   * 標籤為預設品牌
   * 複製
   * 發佈
   * 取消發佈
   * 刪除

   品牌儀表板中的![進階功能表選項](assets/brands-6.png)

您現在可以從AI助理功能表的&#x200B;**[!UICONTROL 品牌]**&#x200B;下拉式清單存取品牌指南。 這可讓AI助理產生符合您規格的內容和資產。 [進一步瞭解AI小幫手](../content/generative-gs.md)

您也可以使用品牌指引來評估內容品質和品牌一致性。 [進一步瞭解內容品質驗證](brands-score.md#validate-quality)

![AI助理功能表與品牌下拉式清單](assets/brands_6.png)

### 設定預設品牌 {#default-brand}

您可以指定預設品牌，在建立行銷活動期間產生內容及計算一致性分數時自動套用。

若要設定預設品牌，請移至您的&#x200B;**[!UICONTROL 品牌]**&#x200B;儀表板。 按一下![](assets/do-not-localize/Smock_More_18_N.svg)圖示並選取&#x200B;**[!UICONTROL 標籤為預設品牌]**，以開啟進階功能表。

品牌儀表板中的![進階功能表選項](assets/brands-6.png)

