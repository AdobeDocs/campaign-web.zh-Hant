---
audience: end-user
title: 選取現有對象
description: 了解如何選取對象
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 33%

---


# 選取現有對象 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="選取現有對象"
>abstract="瀏覽清單以選取現有對象。使用「顯示篩選器」圖示篩選清單，或選取特定資料夾。"

本節說明在定義傳送的目標母體時，如何選取現有的對象。 定義傳送的主要目標時，您也可以：
* [建立一次性對象](one-time-audience.md) 使用查詢模型工具。
* [從外部檔案載入對象](file-audience.md) （僅適用於電子郵件）。

可在傳遞中鎖定的對象，可從 **對象** 左側功能表。 它們源自於多個來源，例如使用者端主控台、Campaign Web對象工作流程或Adobe Experience Platform。 [進一步了解對象](manage-audience.md)

若要為您的訊息選取現有對象，請依照以下步驟進行：

1. 從 **對象** 傳遞建立助理的區段，按一下 **[!UICONTROL 選取對象]** 按鈕，然後選擇 **[!UICONTROL 選取對象]**.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

1. 此畫面會顯示目前資料夾的所有現有對象。

   ![](assets/create-audience2.png){zoomable=&quot;yes&quot;}

   若要從Adobe Experience Platform選擇對象，請瀏覽至 `AEP Audiences folder` 從熒幕的篩選區段中。 [深入瞭解Adobe Experience Platform對象](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable=&quot;yes&quot;}

1. 篩選區段可讓您存取篩選選項，以調整對象清單。 若要這麼做，請按一下 **新增規則** 以存取「查詢建模工具」，這可讓您為對象清單建立進階篩選器。 [瞭解如何使用查詢模型工具](../query/query-modeler-overview.md)

   例如，您可以定義規則以篩選對象的來源，如下所示：

   ![](assets/filter-on-aep-audience.png){zoomable=&quot;yes&quot;}

1. 按一下 **確認** 將您的對象新增為傳送主要目標。 完成後，您仍然可以使用查詢塑模工具，透過按一下 **編輯規則** 按鈕。

   ![](assets/refine-audience.png){zoomable=&quot;yes&quot;}

   您也可以設定控制組來測量行銷活動的影響。控制組不會收到訊息。可讓您將收到訊息之母體的行為與未收到訊息之聯絡人的行為進行比較。[了解更多](control-group.md)
