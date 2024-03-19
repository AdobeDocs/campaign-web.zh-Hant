---
audience: end-user
title: 使用調解工作流程活動
description: 瞭解如何使用協調工作流程活動
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 40%

---

# 調和 {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="調和活動"
>abstract="**調和**&#x200B;活動是&#x200B;**目標定位**&#x200B;活動，它可讓您定義 Adobe Campaign 資料庫資料與工作表資料之間的連結。例如，可以將&#x200B;**調和**&#x200B;活動放在&#x200B;**載入檔案**&#x200B;活動之後，以將非標準資料匯入資料庫。在此情況下，**調和**&#x200B;活動可讓您定義 Adobe Campaign 資料庫資料與外部資料表資料之間的連結。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="調和選取欄位"
>abstract="調和選取欄位"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="調和建立條件"
>abstract="調和建立條件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="調和產生補充"
>abstract="調和產生補充"

此 **調解** 活動是 **目標定位** 活動可讓您定義Adobe Campaign資料庫中的資料與工作表格中的資料（例如從外部檔案載入的資料）之間的連結。

例如，可以將&#x200B;**調和**&#x200B;活動放在&#x200B;**載入檔案**&#x200B;活動之後，以將非標準資料匯入資料庫。在此案例中， **調解** 活動可讓您定義Adobe Campaign資料庫中的資料與工作表中的資料之間的連結。

## 最佳實務 {#reconciliation-best-practices}

當 **擴充** 活動可讓您定義要在工作流程中處理的其他資料(您可以使用 **擴充** 活動以合併來自多組資料，或建立臨時資源的連結)， **調解** 活動可讓您將未識別的資料連結至現有資源。

>[!NOTE]
>調解作業表示連結維度的資料已在資料庫中。  例如，如果您匯入購買檔案，顯示何時購買了哪些產品、哪個客戶等，則產品和客戶必須已存在於資料庫中。

## 設定調和活動 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="目標定位維度"
>abstract="選取新的目標定位維度。維度可讓您定義目標族群：收件者、應用程式訂閱者、操作者、訂閱者等。預設會選取目前的目標定位維度。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="調和規則"
>abstract="選取要用於重複資料刪除的調解規則。 若要使用屬性，請選取 **簡單屬性** 選項，然後選擇來源和目的地欄位。 若要使用查詢建模程式建立自己的調解條件，請選取 **進階調解條件** 選項。"
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="使用查詢建模工具"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="選取目標定位維度"
>abstract="選取要調和之輸入資料的目標定位維度。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=zh-Hant#targeting-dimensions" text="目標定位維度"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="保留未調和的資料"
>abstract="依預設，未調和的資料保留在傳出轉變中，並可在工作表中供未來使用。若要移除未調和的資料，請停用「**保留未調和的資料**」選項。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="調和屬性"
>abstract="選取用於調和資料的屬性，然後按一下「確認」。"

請依照下列步驟設定 **調解** 活動：

1. 拖放 **調解** 活動放入工作流程。 此活動應在包含母體的轉變之後新增，其母體的目標維度不會直接來自Adobe Campaign。

1. 選取新的目標定位維度。維度可讓您定義目標族群：收件者、應用程式訂閱者、操作者、訂閱者等。[進一步瞭解目標維度](../../audience/about-recipients.md#targeting-dimensions).

1. 選取要用於調解的欄位。 您可以使用一個或多個調和標準。

   1. 若要使用屬性來調解資料，請選取 **簡單屬性** 選項。 此 **來源** 欄位列出輸入轉變中可用的欄位，這些欄位要協調。 此 **目的地** 欄位與所選目標維度的欄位相對應。 當來源和目的地相等時，資料就會進行協調。 例如，選取 **電子郵件** 根據設定檔的電子郵件地址進行重複資料刪除的欄位。

      若要新增其他調解條件，請按一下 **新增規則** 按鈕。 如果指定了多個連線條件，則必須全部驗證這些條件，才能將資料連結在一起。

      ![](../assets/workflow-reconciliation-criteria.png)

   1. 若要使用其他屬性來調解資料，請選取 **進階調解條件** 選項。 然後，您可以使用查詢建模器建立自己的調解條件。 [瞭解如何使用查詢建模器](../../query/query-modeler-overview.md).

1. 您可以使用來篩選要調解的資料 **建立篩選器** 按鈕。 這可讓您使用查詢建模器建立自訂條件。 [瞭解如何使用查詢建模器](../../query/query-modeler-overview.md)

依預設，未調解的資料會保留在出站轉變中，並可在工作表中供未來使用。 若要移除未調和的資料，請停用「**保留未調和的資料**」選項。

## 範例 {#reconciliation-example}

下列範例會示範一個工作流程，其會從包含新客戶之匯入檔案直接建立設定檔對象。它由下列活動組成：

工作流設計如下：

![](../assets/workflow-reconciliation-sample-1.0.png)


它是透過以下活動建置：

* [載入檔案](load-file.md)活動會上傳包含從外部工具擷取之設定檔資料的檔案。

  例如：

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **調解** 使用將傳入資料識別為設定檔的活動 **電子郵件** 和 **出生日期** 做為調解條件的欄位。

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [儲存對象](save-audience.md) 根據這些更新建立新對象的活動。 您也可以取代 **儲存對象** 活動，按 **結束** 活動（若不需要建立或更新特定對象）。 收件者設定檔會在您執行工作流程時進行更新。


## 相容性 {#reconciliation-compat}

此 **調解** 使用者端主控台中沒有活動。 全部 **擴充功能** 在啟用調解選項的使用者端主控台中建立的活動會顯示為 **調解** Campaign網頁使用者介面中的活動。
