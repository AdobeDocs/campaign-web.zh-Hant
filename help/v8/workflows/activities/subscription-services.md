---
audience: end-user
title: 使用訂閱服務活動
description: 瞭解如何使用訂閱服務工作流程活動
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 9cd2d3c7ac4c0ff3c9939cd43606400011fce739
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 17%

---

# 訂閱服務 {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="訂閱服務活動"
>abstract="「訂閱服務」活動允許在單一動作中訂閱或取消訂閱多個設定檔。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="訂閱服務一般參數"
>abstract="選擇所需的服務並選擇要執行的動作 (訂閱或取消訂閱)。將「**傳送確認訊息**」選項切換為開啟，通知族群他們正訂閱或取消訂閱所選服務。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="產生傳出轉變"
>abstract="切換「**產生傳出轉變**」選項，可在活動之後新增轉變。"

此 **訂閱服務** 活動是 **資料管理** 活動。 它可讓您為轉變中指定的母體建立或刪除資訊服務的訂閱。

## 設定訂閱服務活動 {#subscription-services-configuration}

請依照下列步驟設定 **訂閱服務** 活動：

1. 新增 **訂閱服務** 活動放入工作流程。 在鎖定設定檔目標或匯入包含已識別資料的檔案後，您可以使用此活動。

1. 使用以下其中一個選項，選取您要管理訂閱的服務：

   * **[!UICONTROL 選取特定服務]**：手動選取服務，使用 **[!UICONTROL 服務]** 欄位。

   * **[!UICONTROL 從入站轉變]**：使用入站轉變中指定的服務。 例如，您可以匯入指定每行所管理之服務的檔案。接著會為每個設定檔動態選取要對其執行操作的服務。

   ![](../assets/workflow-subscription-service.png)

1. 選取要執行的作業： **訂閱** 或 **取消訂閱**.

   如果服務是在入站轉變中定義，您可以選擇如何擷取此作業：

   * **選取特定作業型別**：手動選取要執行的操作(**訂閱** 或 **取消訂閱**)

   * **從入站轉變的路徑中選取操作型別**：選取輸入資料的欄，並指定為每個記錄執行的操作。 例如，您可以匯入一個檔案，該檔案指定對「operation」欄中的每一行執行的操作。

     >[!NOTE]
     >
     >此處只能選取布林值或整數欄位。 請確定包含要執行之作業的資料符合此格式。 例如，如果您是從「載入檔案」活動載入資料，請檢查您是否已正確設定包含此作業之欄的格式 **[!UICONTROL 載入檔案]** 活動。 範例顯示於 [本節](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. 若要通知收件者他們已訂閱或取消訂閱所選服務，請切換 **[!UICONTROL 傳送確認訊息]** 選項開啟。 此通知的內容是在與資訊服務相關的傳遞範本中定義的。

1. 如果您使用來自入站轉變的資料，會 **[!UICONTROL 其他資訊]** 區段隨即顯示，您可在此指定每個記錄的資料與訂閱來源。 您可以將此區段保留空白，這樣在執行工作流程時就不會設定日期或來源。

   * 如果傳入資料包含一欄，指出服務設定檔的訂閱日期，則可在 **[!UICONTROL 日期]** 欄位。

   * 在 **[!UICONTROL 來源路徑]** 欄位，定義訂閱的來源。 您可以核取「 」，將其設為輸入資料的其中一個欄位，或設為您選取的常數值 **[!UICONTROL 將常數設定為原點]** 選項。

   ![](../assets/workflow-subscription-service-additional.png)

1. 若要在活動後新增出站轉變，請切換 **[!UICONTROL 產生出站轉變]** 選項開啟。

## 範例 {#example}

### 將對象訂閱至特定服務 {#uc1}

以下工作流程說明如何將受眾訂閱現有服務。

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL 建立對象]** 活動會鎖定現有對象。

* A **[!UICONTROL 訂閱服務]** 活動可讓您選取必須訂閱設定檔的服務。

<!--
### Updating multiple subscription statuses from a file {#uc2}

The workflow below shows how to import a file containing profiles and update their subscription to several services specified in the file.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Load file]** activity loads a CSV file containing the data and defines the structure of the imported columns. The "service" and "operation" columns specify the service to update and the operation to perform (subscription or unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  As you may have noticed, the operation is specified in the file as "sub" or "unsub". The system expects a **Boolean** or **Integer** value to recognize the operation to perform: "0" to unsubscribe and "1" to subscribe. To match this requirement, a remapping of values must be performed in the detail of the "operation" column in the sample file configuration screen.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  If your file already uses "0" and "1" to identify the operation, you don't need to remap those values. Only make sure that the column is processed as a **Boolean** or **Integer** in the sample file columns.

* A **[!UICONTROL Reconciliation]** activity identifies the data from the file as belonging to the profile dimension of the Adobe Campaign database. The **email** field of the file is matched to the **email** field of the profile resource.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL Enrichment]** activity creates a link to the "Services (nms)" table and creates a simple join between the "service" column of the uploaded file, and the services "internal name" field in the database.

    ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplication]** based on the **email** field identifies duplicates. It is important to eliminate duplicates since the subscription to a service will fail for all data in case of duplicates.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)
  
* A **[!UICONTROL Subscription Services]** identifies the services to update as coming from the transition, through the link created in the **[!UICONTROL Reconciliation]** activity.

  The **[!UICONTROL Operation type]** is identified as coming from the **operation** field of the file. Only Boolean or Integer fields can be selected here. If the column of your file that contains the operation to perform does not appear in the list, make sure that you have correctly set your column format in the **[!UICONTROL Load file]** activity, as explained earlier in this example.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)-->
