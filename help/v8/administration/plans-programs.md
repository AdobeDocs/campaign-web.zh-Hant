---
audience: end-user
title: 計劃和專案
description: 瞭解如何在Adobe Campaign中建立和設定計畫和方案
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 10%

---

# 計劃和專案 {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="計劃和專案"
>abstract="您現在可在 Campaign Web 使用者介面中設定行銷計劃和專案的資料夾階層。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hant" text="請參閱版本注意事項"

Adobe Campaign 讓您可以為行銷計劃和專案設定資料夾階層。

為了更妥善地組織這些活動，Adobe建議使用下列階層：計畫`>`方案`>`行銷活動

* **計畫**&#x200B;可能包含多個計畫。 它會定義一段時間的策略目標。
* **方案**&#x200B;可能包含其他方案，以及行銷活動、工作流程和登入頁面。
* **行銷活動**&#x200B;可能包含傳遞、工作流程和登入頁面。

## 建立及設定計畫 {#create-plan}

若要建立計畫，您必須建立資料夾型別為&#x200B;**[!UICONTROL 計畫]** [深入瞭解如何建立資料夾](../get-started/work-with-folders.md)。

![](assets/plan_create.png){zoomable="yes"}

前往您計畫的&#x200B;**[!UICONTROL 資料夾設定]**&#x200B;來管理它。

![](assets/plan_settings.png){zoomable="yes"}

您可以定義&#x200B;**[!UICONTROL 自訂選項]**，並設定計畫的排程日期。

![](assets/plan_options.png){zoomable="yes"}

若要管理&#x200B;**[!UICONTROL 自訂選項]**：

1. 瀏覽至&#x200B;**[!UICONTROL 結構描述]**
1. 選擇篩選器中的&#x200B;**[!UICONTROL 可編輯]**&#x200B;結構描述
1. 按一下&#x200B;**[!UICONTROL 編輯自訂詳細資料]**&#x200B;的圖示

![](assets/plan_edit.png){zoomable="yes"}

您可以進行下列設定：

![](assets/plan_customfields.png){zoomable="yes"}

## 建立及設定程式

若要在您的計畫中建立方案（[深入瞭解如何建立方案](#create-plan)），您必須加入您的計畫，並建立資料夾型別為&#x200B;**[!UICONTROL 方案]** [深入瞭解如何建立資料夾](../get-started/work-with-folders.md)。

![](assets/program_create.png){zoomable="yes"}

移至程式的&#x200B;**[!UICONTROL 資料夾設定]**&#x200B;來管理它。

![](assets/program_settings.png){zoomable="yes"}

您可以定義&#x200B;**[!UICONTROL 自訂選項]**，並設定程式的排程日期。

![](assets/program_options.png){zoomable="yes"}

若要管理&#x200B;**[!UICONTROL 自訂選項]**：

1. 瀏覽至&#x200B;**[!UICONTROL 結構描述]**
1. 選擇篩選器中的&#x200B;**[!UICONTROL 可編輯]**&#x200B;結構描述
1. 按一下&#x200B;**[!UICONTROL 編輯自訂詳細資料]**&#x200B;的圖示

![](assets/program_edit.png){zoomable="yes"}

您可以進行下列設定：

![](assets/program_customfields.png){zoomable="yes"}

## 如何將行銷活動連結至方案

您有兩種方式可將行銷活動連結至方案：

### 方式#1：您已擁有方案，且想要建立與其連結的行銷活動

若要將新行銷活動連結至您的方案，請直接在方案中建立您的行銷活動：

![](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL 資料夾]**&#x200B;設定會自動以您程式的路徑歸檔。

![](assets/program_campaign_folder.png){zoomable="yes"}

### 方式#2：您已有現有行銷活動，且想將其連結至現有方案

前往您要連結至方案之行銷活動的&#x200B;**[!UICONTROL 設定]**&#x200B;按鈕：

![](assets/campaign_settings.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 屬性]**&#x200B;中，按一下&#x200B;**[!UICONTROL 資料夾]**&#x200B;設定中的&#x200B;**[!UICONTROL 資料夾]**&#x200B;圖示，以選擇您的&#x200B;**[!UICONTROL 程式]**&#x200B;資料夾。

![](assets/campaign_folder.png){zoomable="yes"}

選取您的&#x200B;**[!UICONTROL 程式]**&#x200B;資料夾，然後按一下&#x200B;**[!UICONTROL 確認]**&#x200B;按鈕，再按一下&#x200B;**[!UICONTROL 儲存並關閉]**&#x200B;按鈕。

![](assets/campaign_linked.png){zoomable="yes"}

您的行銷活動現在已列在您的方案中：

![](assets/campaign_in_program.png){zoomable="yes"}
