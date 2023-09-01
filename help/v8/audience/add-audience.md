---
audience: end-user
title: 選取現有對象
description: 了解如何選取對象
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 57%

---


# 選取現有對象 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="選取現有對象"
>abstract="瀏覽清單以選取現有對象。 使用「顯示篩選器」圖示來篩選清單，或選取特定資料夾。"

本章節說明如何在定義電子郵件傳遞的目標母體時選取現有對象。

您也可以：

* 建立新對象。 [了解更多](segment-builder.md)
* 從外部檔案載入對象（僅適用於電子郵件）。 [了解更多](file-audience.md)
* 使用 Adobe Experience Platform 對象。[了解更多](aep-audience.md)。


若要為您的訊息選取現有對象，請依照以下步驟進行：

1. 從傳遞建立助理的「**對象**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

   ![](assets/create-audience.png)

1. 選擇「**[!UICONTROL 選取對象]**」以使用現有對象。若要建立新對象用於此電子郵件，請選擇「**建立您自己的**」。請參閱本[章節](segment-builder.md)。

   此畫面會顯示目前資料夾的所有現有對象。

   ![](assets/create-audience2.png)

   建立對象是從 **對象** 左側功能表。 也可在使用者端主控台中建立。

   若要使用Adobe Experience Platform受眾，您需要設定與目的地的整合。 請參閱 [Adobe Experience Platform目標檔案](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hant){target="_blank"}.

1. 選擇對象，然後按一下「**選取**」。
1. 使用 **顯示篩選器** 圖示來顯示篩選選項。 按一下 **新增規則** 若要存取規則產生器：使用規則產生器，可讓您為對象清單建立進階篩選器。 在此瞭解如何使用規則產生器 [區段](segment-builder.md).

   ![](assets/create-audience4.png)

1. 按一下「**儲存**」。

您也可以設定控制組來測量行銷活動的影響。控制組不會收到訊息。可讓您將收到訊息之母體的行為與未收到訊息之聯絡人的行為進行比較。若要了解詳細資訊，請參閱[本章節](control-group.md)。