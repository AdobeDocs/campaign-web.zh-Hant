---
audience: end-user
title: 使用變更資料來源工作流程活動
description: 瞭解如何使用變更資料來源工作流程活動
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---

# 變更資料來源 {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="變更資料來源"
>abstract="您可以使用&#x200B;**變更資料來源**&#x200B;活動為工作流程的工作表選取不同的資料來源。"

**變更資料來源**&#x200B;活動是&#x200B;**鎖定目標**&#x200B;活動。 此活動可讓您變更工作流程工作表使用的資料來源。 這可讓您跨不同的資料庫管理資料並改善效能，進而提供更大的彈性。

在工作流程中，透過轉換從一個活動傳輸到另一個活動的資料會儲存在暫時&#x200B;**工作表格**&#x200B;中。 依照預設，工作表格會建立在與已處理資料來源相同的資料庫中。 例如，查詢「設定檔」表格（儲存在雲端資料庫上）時，會在相同的雲端資料庫上建立「工作」表格。

在某些情況下，目前的資料庫中可能沒有資料，或是資料執行效率不夠高，無法執行單一作業。 因此，您可能需要藉由新增&#x200B;**[!UICONTROL 變更資料來源]**&#x200B;活動，強制工作流程使用不同的資料庫來執行這類作業。

有關Campaign架構的詳細資訊，請參閱[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)。

>[!IMPORTANT]
>
>請注意，不應將&#x200B;**[!UICONTROL 變更維度]**&#x200B;和&#x200B;**[!UICONTROL 變更資料來源]**&#x200B;活動新增到一列。 如果您需要連續使用這兩個活動，請在它們之間加入&#x200B;**[!UICONTROL 擴充]**&#x200B;活動。 這可確保正確執行並防止潛在的衝突或錯誤。

>[!NOTE]
>
>**變更資料Source**&#x200B;活動最多可以在每次執行時處理一百萬筆記錄。 如果您需要提高此上限，請聯絡您的Adobe代表。

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## 設定變更資料來源活動 {#configure}

請依照下列步驟設定&#x200B;**變更資料來源**&#x200B;活動：

![熒幕擷圖顯示如何將[變更資料來源]活動新增至工作流程。](../assets/workflow-change-data-source-add.png)

1. 新增&#x200B;**變更資料來源**&#x200B;活動至您的工作流程。

1. 定義您要移動工作表格的資料來源：

   * **[!UICONTROL 預設Campaign資料庫(PostgreSQL)]**：使用預設的Campaign本機資料庫。
   * **[!UICONTROL FDA外部帳戶]**：使用透過同盟資料存取功能連線到Adobe Campaign的外部雲端資料庫。

     >[!AVAILABILITY]
     >
     >Campaign 設定以及與外部系統的連線僅限進階使用者使用，且僅適用於用戶端主控台。[了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hant){target="_blank"}

1. 設定您的工作流程，以使用新資料來源執行所需的作業。

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->