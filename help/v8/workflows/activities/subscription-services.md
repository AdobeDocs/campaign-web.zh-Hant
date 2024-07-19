---
audience: end-user
title: 使用訂閱服務活動
description: 瞭解如何使用訂閱服務工作流程活動
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 0e5b5e916309b2a337ac86f3741bcb83237b3fad
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 18%

---

# 訂閱服務 {#subscription-services}

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

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="其他資訊"
>abstract="其他資訊"

**訂閱服務**&#x200B;活動是&#x200B;**資料管理**&#x200B;活動。 它可讓您為轉變中指定的母體建立或刪除資訊服務的訂閱。

## 設定訂閱服務活動 {#subscription-services-configuration}

請依照下列步驟設定&#x200B;**訂閱服務**&#x200B;活動：

1. 將&#x200B;**訂閱服務**&#x200B;活動新增至您的工作流程。 在鎖定設定檔目標或匯入包含已識別資料的檔案後，您可以使用此活動。

1. 使用以下其中一個選項，選取您要管理訂閱的服務：

   * **[!UICONTROL 選取特定服務]**：使用&#x200B;**[!UICONTROL 服務]**&#x200B;欄位手動選取服務。

   * **[!UICONTROL 來自入站轉變]**：使用在入站轉變中指定的服務。 例如，您可以匯入指定每行所管理之服務的檔案。接著會為每個設定檔動態選取要對其執行操作的服務。

   ![](../assets/workflow-subscription-service.png)

1. 選取要執行的作業： **訂閱**&#x200B;或&#x200B;**取消訂閱**。

   如果服務是在入站轉變中定義，您可以選擇如何擷取此作業：

   * **選取特定作業型別**：手動選取要執行的作業（**訂閱**&#x200B;或&#x200B;**取消訂閱**）

   * **從入站轉變的路徑中選取作業型別**：選取入站資料的資料行，該資料行指定為每個記錄執行的作業。 例如，您可以匯入一個檔案，該檔案指定對「operation」欄中的每一行執行的操作。

     此處只能選取布林值或整數欄位。 請確定包含要執行之作業的資料符合此格式。 例如，如果您是從「載入檔案」活動載入資料，請檢查您是否已在&#x200B;**[!UICONTROL 載入檔案]**&#x200B;活動中正確設定包含作業的資料行格式。 在[此區段](#uc2)中呈現範例。

     >[!CAUTION]
     >
     >依預設，如果您選取此選項，**訂閱服務**&#x200B;活動預期會有一個連結定義，指向工作流程中設定的&#x200B;**服務(nms)**&#x200B;資料表。 若要這麼做，請確保您已在工作流程中向上設定&#x200B;**擴充活動**&#x200B;中的調解連結。 [此處](#uc2)提供如何使用此選項的範例。

   ![](../assets/workflow-subscription-service-inbound.png)

1. 若要通知收件者他們已訂閱或取消訂閱選取的服務，請開啟&#x200B;**[!UICONTROL 傳送確認訊息]**&#x200B;選項。 此通知的內容是在與資訊服務相關的傳遞範本中定義的。

1. 如果您使用來自入站轉變的資料，則會顯示&#x200B;**[!UICONTROL 其他資訊]**&#x200B;區段，讓您指定每個記錄的資料和訂閱來源。 您可以將此區段保留空白，這樣在執行工作流程時就不會設定日期或來源。

   * 如果傳入資料包含一欄，指出服務設定檔的訂閱日期，您可以在&#x200B;**[!UICONTROL 日期]**&#x200B;欄位中選取它。

   * 在&#x200B;**[!UICONTROL 原始路徑]**&#x200B;欄位中，定義訂閱的來源。 您可以核取&#x200B;**[!UICONTROL 將常數設定為來源]**&#x200B;選項，將其設定為輸入資料的其中一個欄位，或設定為您選擇的常數值。

   ![](../assets/workflow-subscription-service-additional.png)

1. 若要在活動後新增出站轉變，請開啟&#x200B;**[!UICONTROL 產生出站轉變]**&#x200B;選項。

## 範例 {#example}

### 將對象訂閱至特定服務 {#uc1}

以下工作流程說明如何將受眾訂閱現有服務。

![](../assets/workflow-subscription-service-uc1.png)

* **[!UICONTROL 建置對象]**&#x200B;活動會鎖定現有對象。

* **[!UICONTROL 訂閱服務]**&#x200B;活動可讓您選取必須訂閱設定檔的服務。

### 從檔案更新多個訂閱狀態 {#uc2}

以下工作流程說明如何匯入包含設定檔的檔案，並將其訂閱更新為檔案中指定的數個服務。

![](../assets/workflow-subscription-service-uc2.png)

* **[!UICONTROL 載入檔案]**&#x200B;活動載入包含資料的CSV檔案，並定義匯入資料行的結構。 「服務」和「作業」欄指定要更新的服務及要執行的作業（訂閱或取消訂閱）。

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  如您所注意的，此操作在檔案中指定為 &quot;sub&quot; 或 &quot;unsub&quot;。此系統需要一個 **Boolean** 或 **Integer** 整數值來識別要執行的操作：&quot;0&quot; 為取消訂閱與 &quot;1&quot; 為訂閱。若要符合此需求：
   * 「作業」資料行的&#x200B;**資料型別**&#x200B;已設定為整數。
   * 必須執行&#x200B;**值重新對應**，以比對&quot;sub&quot;和&quot;unsub&quot;值與&quot;1&quot;和&quot;0&quot;值。

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  如果您的檔案已使用 &quot;0&quot; 及 &quot;1&quot; 來識別此操作，則不需要重新映射這些值。僅確定在範例檔案資料行中，資料行是以&#x200B;**Boolean**&#x200B;或&#x200B;**Integer**&#x200B;處理。

* **[!UICONTROL 調解]**&#x200B;活動會將檔案中的資料識別為屬於Adobe Campaign資料庫的設定檔維度。 檔案的&#x200B;**電子郵件**&#x200B;欄位與設定檔資源的&#x200B;**電子郵件**&#x200B;欄位相符。

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* **[!UICONTROL 擴充]**&#x200B;活動會建立與「服務(nms)」表格的調解連結，上傳檔案的「服務」欄與資料庫中的服務「內部名稱」欄位之間具有簡單聯結。

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* **[!UICONTROL 訂閱服務]**&#x200B;將要更新的服務識別為來自轉換。

  **[!UICONTROL 作業型別]**&#x200B;被識別為來自檔案的&#x200B;**作業**&#x200B;欄位。 此處只能選取 Boolean 或 Integer 欄位。如果檔案中包含要執行的操作欄未出現在清單中，請確保您已正確設定&#x200B;**[!UICONTROL 載入檔案]**&#x200B;活動中的欄格式，如本範例前面所述。

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
