---
audience: end-user
title: 使用 Adobe Experience Platform 對象
description: 了解如何使用 Adobe Experience Platform 對象
badge: label="Beta"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 32%

---

# 使用 Adobe Experience Platform 對象{#aep-audience}

Adobe Campaign受管理的Cloud Service目標和來源聯結器可緊密整合Adobe Campaign和Adobe Experience Platform。

建立Adobe Experience Platform受眾並可在使用者端主控台中使用後，您就可以像使用Campaign受眾一樣使用該受眾，以個人化及傳送訊息。

>[!NOTE]
>
>若要在Campaign中使用Adobe Experience Platform受眾，您需要設定與Adobe來源和目標的整合。 請參閱 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

若要選取傳送的對象，您也可以：

* 建立新對象。 [了解更多](../query/query-modeler-overview.md)
* 從外部檔案載入對象。 [了解更多](file-audience.md)
* 使用現有的Campaign對象。 [了解更多](add-audience.md)。

若要選取要傳送的Adobe Experience Platform對象，請遵循下列步驟：

1. 從傳遞建立助理的「**對象**」區段，按一下「**[!UICONTROL 選取對象]**」按鈕。

   ![](assets/create-audience.png)

1. 選擇「**[!UICONTROL 選取對象]**」以使用現有對象。若要建立新對象用於此電子郵件，請選擇「**建立您自己的**」。請參閱本[章節](../query/query-modeler-overview.md)。

   此畫面會顯示目前資料夾在Adobe Campaign使用者端主控台中定義的所有現有對象。 若要從Adobe Experience Platform選擇對象，請瀏覽至 `AEP Audiences folder` 從熒幕的篩選區段中。

   ![](assets/select-audience-folder.png)

   您也可以定義規則以根據對象的來源進行篩選，如下所示：

   ![](assets/filter-on-aep-audience.png)

1. 選擇對象，然後按一下「**選取**」。

1. 如果你想要調整您的對象，請按一下「**編輯規則**」。

   ![](assets/refine-audience.png)

1. 使用查詢模型工具，您可以透過其他篩選器或結合不同對象來豐富您的對象。 請參閱本[章節](../query/query-modeler-overview.md)。

1. 按一下「**儲存**」。
