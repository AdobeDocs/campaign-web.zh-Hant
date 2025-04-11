---
audience: end-user
title: 使用資料夾
description: 了解如何在 Adobe Campaign 中管理資料夾
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 25%

---

# 使用資料夾 {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="資料夾屬性"
>abstract="資料夾屬性"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="資料夾安全性"
>abstract="資料夾安全性"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="資料夾限制"
>abstract="資料夾限制"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="資料夾排程"
>abstract="資料夾排程"

## 關於資料夾 {#about-folders}

資料夾是 Adobe Campaign 中的物件，可讓您組織元件和資料。

您可以在導覽樹狀結構中建立、重新命名、重新排序和移動資料夾。您也可以根據您的許可權刪除這些專案。

![顯示資料夾組織的資料夾介面](assets/folders.png){zoomable="yes"}

您可以設定資料夾類型。例如，傳遞的資料夾。 資料夾圖示會依其型別而變更。

## 建立新資料夾 {#create-a-folder}

若要在 Adobe Campaign Web UI 中建立新資料夾，請執行下列步驟：

1. 在&#x200B;**[!UICONTROL Explorer]**&#x200B;中，移至您要建立新資料夾的資料夾。 在&#x200B;**[!UICONTROL ...]**&#x200B;功能表下，選取&#x200B;**[!UICONTROL 建立新資料夾]**。

![在Explorer功能表中建立新資料夾選項](assets/folder_create.png){zoomable="yes"}

當您建立新資料夾時，資料夾型別會預設為父資料夾的型別。 在此範例中，會在&#x200B;**[!UICONTROL 傳送]**&#x200B;資料夾中建立資料夾。

![在傳遞資料夾](assets/folder_new.png){zoomable="yes"}下建立的新資料夾

1. 如有需要，請按一下資料夾型別圖示來變更資料夾型別，然後從顯示的清單中選取所需的型別，如下所示：

![資料夾型別選擇介面](assets/folder_type.png){zoomable="yes"}

按一下&#x200B;**[!UICONTROL 確認]**&#x200B;按鈕以設定資料夾型別。

如果您想建立不含特定型別的資料夾，請選取&#x200B;**[!UICONTROL 一般資料夾]**&#x200B;型別。

您也可以[在 Adobe Campaign 控制台中建立和管理資料夾](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/config/configuration/folders-and-views)。

## 重新排序資料夾 {#reorder-folders}

您可以根據需求重新排序資料夾。 若要這麼做，請按一下&#x200B;**[!UICONTROL 重新排序資料夾]**，如下所示。

在此範例中，**傳送**&#x200B;資料夾包含四個子資料夾。

![顯示資料夾階層的重新排序資料夾介面](assets/folder-reorder.png){zoomable="yes"}

您可以透過&#x200B;**拖放**&#x200B;或使用&#x200B;**上下箭頭**&#x200B;來變更資料夾的順序。

![資料夾重新排序的拖放功能](assets/folder-draganddrop.png){zoomable="yes"}

## 刪除資料夾 {#delete-a-folder}

>[!CAUTION]
>
>刪除資料夾時，儲存於該資料夾的所有資料也會被刪除。

若要刪除資料夾，請在&#x200B;**[!UICONTROL Explorer]**&#x200B;樹狀結構中選取該資料夾，然後按一下&#x200B;**[!UICONTROL ...]**&#x200B;功能表。 選擇「**[!UICONTROL 刪除資料夾]**」。

在Explorer功能表中![刪除資料夾選項](assets/folder_delete.png){zoomable="yes"}

## 資料夾中的數值分佈 {#distribution-values-folder}

值的分佈可協助您瞭解表格內某一欄中的值百分比。

若要檢視資料夾中值的分佈，請按照以下說明繼續操作。

例如，在傳遞中，您可能想要知道&#x200B;**管道**&#x200B;欄中的值分佈。

若要取得此資訊，請前往&#x200B;**[!UICONTROL 傳送]**&#x200B;資料夾，然後按一下&#x200B;**[!UICONTROL 設定資料行]**&#x200B;圖示。

在&#x200B;**[!UICONTROL 設定資料行]**&#x200B;視窗中，按一下與您要分析的資料行相關的&#x200B;**[!UICONTROL 資訊]**&#x200B;圖示。 接著，點擊&#x200B;**[!UICONTROL 「值的分佈」]**&#x200B;按鈕。

![傳遞的值分佈介面](assets/values_deliveries.png){zoomable="yes"}

您會在&#x200B;**[!UICONTROL 管道]**&#x200B;欄中看到值的百分比。

![頻道資料行](assets/values_percentage.png){zoomable="yes"}中值的百分比分佈

>[!NOTE]
>
>對於具有許多值的欄，只會顯示前20個值。 通知&#x200B;**[!UICONTROL 部分載入]**&#x200B;會警告您。

您也可以檢視連結值的分佈。

在屬性清單中，點擊所需連結旁邊的&#x200B;**「+」**&#x200B;按鈕，如下所示。這會將連結新增到&#x200B;**[!UICONTROL 「輸出欄」]**&#x200B;中。您現在可以存取&#x200B;**[!UICONTROL 資訊]**&#x200B;圖示，讓您檢視其值的分佈。 如果您不想在&#x200B;**[!UICONTROL 輸出資料行]**&#x200B;中保留連結，請按一下&#x200B;**[!UICONTROL 取消]**&#x200B;按鈕。

![輸出資料行中連結值的分佈](assets/values_link.png){zoomable="yes"}

您也可以檢視查詢模組化工具中值的分佈。 [如需更多詳情，請參閱此處](../query/build-query.md#distribution-of-values-in-a-query)。

### 篩選值 {#filter-values}

在值分佈視窗中使用&#x200B;**[!UICONTROL 進階篩選器]**，即可根據指定的條件篩選結果。

在上面的傳遞清單範例中（顯示每個管道的分發），您可以篩選該清單，以僅顯示狀態為&#x200B;**已完成**&#x200B;的傳遞。

![套用至值分佈的進階篩選器](assets/values_filter.png){zoomable="yes"}