---
audience: end-user
title: 使用Adobe Experience Manager as a Cloud Service管理資產
description: 瞭解如何使用Adobe Experience Manager as a Cloud Service管理內容
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: 8e035bbf92914f17607a15c184ecf48f5c0efb13
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 使用[!DNL Adobe Experience Manager as a Cloud Service]管理範本{#aem-assets}

## 開始使用 [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

Adobe Campaign網頁介面與Adobe Experience Manager整合，有助於直接在Adobe Experience Manager平台中簡化電子郵件傳遞內容和表單的管理。

![](assets/do-not-localize/book.png)[進一步瞭解Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## 在[!DNL Adobe Experience Manager as a Cloud Service]中建立範本{#create-aem-template}

1. 導覽至您的[!DNL Adobe Experience Manager]作者執行個體，然後按一下頁面左上角的Adobe體驗。 從功能表選擇&#x200B;**[!UICONTROL 網站]**。

1. 存取&#x200B;**[!UICONTROL 行銷活動>品牌名稱>主要區域>頁面名稱]**。

1. 按一下「建立&#x200B;**[!UICONTROL 」]**，然後從下拉式功能表中選取「**[!UICONTROL 頁面]**」。

   ![](assets/aem_1.png)

1. 選取&#x200B;**[!UICONTROL Adobe Campaign電子郵件]**&#x200B;範本，並命名您的Newsletter。

   ![](assets/aem_2.png)

1. 透過新增元件來自訂您的電子郵件內容，例如Adobe Campaign的個人化欄位。 [了解更多](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. 電子郵件準備就緒後，請瀏覽至&#x200B;**[!UICONTROL 頁面資訊]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 開始工作流程]**。

   ![](assets/aem_3.png)

1. 從第一個下拉式清單中，選取&#x200B;**[!UICONTROL 核准Adobe Campaign]**&#x200B;作為工作流程模型，然後按一下&#x200B;**[!UICONTROL 開始工作流程]**。

1. 免責宣告會顯示在您的頁面頂端，顯示`This page is subject to the workflow Approve for Adobe Campaign`。 按一下免責宣告旁的&#x200B;**[!UICONTROL 完成]**&#x200B;以確認檢閱，然後按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/aem_4.png)

1. 再按一下&#x200B;**[!UICONTROL 完成]**，然後在&#x200B;**[!UICONTROL 下一個步驟]**&#x200B;下拉式清單中選取&#x200B;**[!UICONTROL 電子報核准]**。

您的Newsletter現已準備就緒，並已在Adobe Campaign中同步。

## 匯入Adobe Experience Manager as a Cloud Service範本{#aem-templates-perso}

當Experience Manager範本在Adobe Campaign Web中成為內容範本後，您就可以識別並合併電子郵件的必要內容，包括個人化。

1. 在Campaign Web中，從&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表，按一下&#x200B;**[!UICONTROL 建立傳遞]**。

1. 在電子郵件範本視窗中，選取內建的&#x200B;**[!UICONTROL 包含AEM內容的電子郵件傳遞]**&#x200B;範本。

   ![](assets/aem_5.png)

1. 輸入傳遞的&#x200B;**[!UICONTROL 標籤]**，並根據您的需求設定其他選項：

   * **[!UICONTROL 內部名稱]**：指派唯一識別碼給傳遞。

   * **[!UICONTROL 資料夾]**：將傳遞儲存在特定資料夾中。

   * **[!UICONTROL 傳遞代碼]**：使用此欄位，根據您自己的命名慣例來組織您的傳遞。

   * **[!UICONTROL 描述]**：指定傳遞的描述。

   * **[!UICONTROL 性質]**：指定用於分類的電子郵件性質。

1. 為您的電子郵件定義&#x200B;**[!UICONTROL 對象]**。 [了解更多](../email/create-email.md#define-audience)

1. 按一下&#x200B;**[!UICONTROL 編輯內容]**。

1. 從&#x200B;**[!UICONTROL 編輯內容]**&#x200B;功能表，按一下&#x200B;**[!UICONTROL 選取AEM內容]**。

   ![](assets/aem_6.png)

1. 瀏覽您的AEM範本，並選取要匯入至Campaign網頁的範本。

   ![](assets/aem_8.png)

1. 請注意，內容不會自動同步。 如果直接在Adobe Experience Manager中變更您的範本，只要選取「重新整理AEM內容」**[!UICONTROL 即可取得最新版本的範本。]**

1. 若要移除Experience Manager與促銷活動之間的連結，或在電子郵件設計工具中進一步個人化您的Experience Manager範本，請按一下[取消AEM內容連結]。****

   ![](assets/aem_9.png)

1. 如果您已將個人化內容新增至您的Experience Manager範本，請按一下[模擬內容] ****，以使用測試設定檔預覽其顯示在訊息中的方式。

[進一步瞭解預覽和測試設定檔](../preview-test/preview-content.md)

1. 檢視訊息預覽時，任何個人化元素都會自動取代為所選測試設定檔中的對應資料。

   如有需要，可以透過&#x200B;**[!UICONTROL 管理測試設定檔]**&#x200B;按鈕新增其他測試設定檔。

您的傳送現已準備就緒，可供傳送。
