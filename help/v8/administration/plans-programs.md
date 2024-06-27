---
audience: end-user
title: 計劃和專案
description: 瞭解如何在Adobe Campaign中建立和設定計畫和方案
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 10%

---

# 計劃和專案 {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="計劃和專案"
>abstract="您現在可在 Campaign Web 使用者介面中設定行銷計劃和專案的資料夾階層。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hant" text="請參閱版本注意事項"

Adobe Campaign 讓您可以為行銷計劃和專案設定資料夾階層。

為了更妥善地組織它們，Adobe建議使用下列階層：計畫 `>` 計畫 `>` 行銷活動

* A **計畫** 可能包含多個程式。 它會定義一段時間的策略目標。
* A **方案** 可能包含其他方案以及行銷活動、工作流程和登入頁面。
* A **行銷活動** 可能包含傳遞、工作流程和登入頁面。

## 建立及設定計畫 {#create-plan}

若要建立計畫，您必須使用資料夾型別建立資料夾 **[!UICONTROL 計畫]** [進一步瞭解建立資料夾](create-manage-folder.md).

![](assets/plan_create.png){zoomable="yes"}

前往 **[!UICONTROL 資料夾設定]** 管理計畫。

![](assets/plan_settings.png){zoomable="yes"}

您可以定義 **[!UICONTROL 自訂選項]**，並設定計畫的排程日期。

![](assets/plan_options.png){zoomable="yes"}

若要管理  **[!UICONTROL 自訂選項]**：

1. 瀏覽至 **[!UICONTROL 方案]**
1. 選擇 **[!UICONTROL 可編輯]** 篩選器中的結構描述
1. 按一下 **[!UICONTROL 編輯自訂詳細資料]**

![](assets/plan_edit.png){zoomable="yes"}

您可以進行下列設定：

![](assets/plan_customfields.png){zoomable="yes"}

## 建立及設定程式

若要在您的計畫中建立方案([深入瞭解如何建立計畫](#create-plan))，您必須加入您的計畫，並以資料夾型別建立資料夾 **[!UICONTROL 計畫]** [進一步瞭解建立資料夾](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

前往 **[!UICONTROL 資料夾設定]** 管理它。

![](assets/program_settings.png){zoomable="yes"}

您可以定義 **[!UICONTROL 自訂選項]**，並設定方案的排程日期。

![](assets/program_options.png){zoomable="yes"}

若要管理  **[!UICONTROL 自訂選項]**：

1. 瀏覽至 **[!UICONTROL 方案]**
1. 選擇 **[!UICONTROL 可編輯]** 篩選器中的結構描述
1. 按一下 **[!UICONTROL 編輯自訂詳細資料]**

![](assets/program_edit.png){zoomable="yes"}

您可以進行設定：

![](assets/program_customfields.png){zoomable="yes"}

## 如何將行銷活動連結至方案

您有兩種方式可將行銷活動連結至方案：

### 方式#1：您已擁有方案，且想要建立與其連結的行銷活動

若要將新行銷活動連結至您的方案，請直接在方案中建立您的行銷活動：

![](assets/program_campaign_create.png){zoomable="yes"}

此 **[!UICONTROL 資料夾]** 設定會自動以您程式的路徑歸檔。

![](assets/program_campaign_folder.png){zoomable="yes"}

### 方式#2：您已擁有現有行銷活動，且想要將其連結至現有方案

前往 **[!UICONTROL 設定]** 連結至方案之促銷活動的按鈕：

![](assets/campaign_settings.png){zoomable="yes"}

在其 **[!UICONTROL 屬性]**，按一下 **[!UICONTROL 資料夾]** 圖示於 **[!UICONTROL 資料夾]** 設定，以便選擇您的 **[!UICONTROL 計畫]** 資料夾。

![](assets/campaign_folder.png){zoomable="yes"}

選取您的 **[!UICONTROL 計畫]** 資料夾並按一下 **[!UICONTROL 確認]** 按鈕，然後開啟 **[!UICONTROL 儲存並關閉]** 按鈕。

![](assets/campaign_linked.png){zoomable="yes"}

您的行銷活動現在已列在您的方案中：

![](assets/campaign_in_program.png){zoomable="yes"}
