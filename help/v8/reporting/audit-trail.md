---
product: campaign
title: 稽核軌跡
description: 瞭解如何使用Campaign稽核軌跡監控您的執行個體
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 稽核軌跡 {#audit-trail}

在Adobe Campaign Web使用者介面中，**[!UICONTROL 稽核軌跡]**&#x200B;功能可讓使用者完全瞭解對執行個體內重要實體所做的所有修改，通常是對執行個體的順利操作產生重大影響的修改。

>[!IMPORTANT]
>
>* Adobe Campaign網頁使用者介面不會稽核使用者許可權、範本、個人化或行銷活動中所做的變更。
>* 只有執行個體的管理員可以管理稽核軌跡。

**[!UICONTROL 稽核軌跡]**&#x200B;功能會持續即時記錄Adobe Campaign執行個體內發生的動作和事件的詳細記錄。 它提供一種便利的方法，用於存取按時間順序排列的資料記錄，解決諸如工作流程狀態、要修改它們的最新個人，或使用者在執行個體內執行的活動等查詢。

+++ 深入瞭解稽核軌跡可用實體

* **Source結構描述稽核軌跡**&#x200B;可讓您在Campaign V8使用者端主控台中監視活動以及最近對結構描述所做的修改。

  如需結構描述的詳細資訊，請參閱[Campaign v8檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas)。

* **工作流程稽核軌跡**&#x200B;可讓您追蹤活動及最近對工作流程所做的變更，包括其目前狀態，例如：

   * 開始
   * 暫停
   * 停止
   * 重新啟動
   * 清除，等於「整個清除」歷程記錄動作
   * 模擬，等於在模擬模式中啟動動作
   * 喚醒，等於「立即執行擱置中的工作」動作
   * 無條件停止

  如需工作流程的詳細資訊，請參閱此[頁面](../workflows/gs-workflows.md)。

* **選項稽核軌跡**&#x200B;可讓您監視活動以及最近對Campaign V8中選項所做的修改。

  如需選項的詳細資訊，請參閱此[頁面](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options)。

* **傳遞稽核軌跡**&#x200B;可讓您檢查活動和對傳遞進行的最後修改。

  如需傳遞的詳細資訊，請參閱此[頁面](../msg/gs-deliveries.md)。

* **外部帳戶**&#x200B;可讓您檢查Campaign V8中對外部帳戶所做的修改，這些修改由技術流程（如技術工作流程或行銷活動工作流程）使用。

  如需外部帳戶的詳細資訊，請參閱此[頁面](../administration/external-account.md)。

* **傳遞對應**&#x200B;可讓您監視活動以及最近對Campaign V8中的傳遞對應所做的修改。

  如需傳遞對應的詳細資訊，請參閱此[頁面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings)。

* **網頁應用程式**&#x200B;可讓您檢查在Campaign V8中對網頁表單所做的修改，這些修改用於建立具有輸入和選擇欄位的頁面，並且可能包含來自資料庫的資料。

  如需網頁應用程式的詳細資訊，請參閱此[頁面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps)。

* **選件**&#x200B;可讓您檢查活動和對您的選件進行的最後修改。

  如需優惠方案的詳細資訊，請參閱此[頁面](../msg/offers.md)。

* **操作員**&#x200B;可讓您監視活動以及最近在Campaign V8中對操作員所做的修改。

  如需運運算元的詳細資訊，請參閱此[頁面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators)。

+++

## 存取稽核軌跡 {#accessing-audit-trail}

若要存取執行個體的&#x200B;**[!UICONTROL 稽核軌跡]**：

1. 在&#x200B;**[!UICONTROL 管理]**&#x200B;功能表下，選取&#x200B;**[!UICONTROL 稽核軌跡]**。

   ![熒幕擷圖顯示[管理]功能表，其中已選取[稽核軌跡]選項](assets/audit-trail-1.png)

1. **[!UICONTROL 稽核軌跡]**&#x200B;視窗會開啟，其中包含您實體的清單。 Adobe Campaign Web使用者介面會稽核工作流程、選項、傳送和結構的建立、編輯和刪除動作。

   選取其中一個實體以深入瞭解最後的修改。

1. **[!UICONTROL 稽核實體]**&#x200B;視窗提供有關所選實體的詳細資訊，例如：

   * **[!UICONTROL 型別]**：工作流程、選項、傳遞或結構描述。
   * **[!UICONTROL 實體]**：活動的內部名稱。
   * **[!UICONTROL 修改者]**：上次修改此實體的人員使用者名稱。
   * **[!UICONTROL 動作]**：此實體上執行的最後一個動作，已建立、已修改或已刪除。
   * **[!UICONTROL 修改日期]**：在此實體上執行最後動作的日期。

   程式碼區塊會針對實體中的確切變更提供詳細資訊。

   ![熒幕擷圖顯示[稽核]實體視窗，其中包含修改詳細資訊](assets/audit-trail-2.png)