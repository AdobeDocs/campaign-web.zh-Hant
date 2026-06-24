---
audience: end-user
title: 使用「結束工作流程」活動
description: 瞭解如何使用結束工作流程活動
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 54%

---

# 結束 {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="結束活動"
>abstract="「**結束**」活動可讓您以圖形方式標記工作流程的終點。 若有多個傳入轉變可供使用，請使用「**要加入的集合**」區段以選取要連接到該活動的轉變。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="要加入的集合"
>abstract="勾選您想要連接的先前活動，作為&#x200B;**結束**&#x200B;活動的傳入轉變。 所選的活動接著會連接到&#x200B;**結束**。 若有多個傳入轉變可以連接到該活動時，才會顯示此區段。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="外部訊號"
>abstract="結束活動參數中外部訊號區段的預留位置。 僅適用於協調的行銷活動。 請勿刪除"

**End**&#x200B;活動是&#x200B;**流量控制**&#x200B;活動。 它可讓您以圖形方式標籤工作流程的結尾。 此活動為選用。

有多個入站轉變可用時，活動可支援多個入站轉變。

在&#x200B;**要聯結**&#x200B;的集合區段中，檢查您先前要連線作為&#x200B;**End**&#x200B;活動之入站轉變的活動。 接著，選取的活動會連結至工作流程畫布中的&#x200B;**End**。

![工作流程重複資料刪除組態程式](../assets/workflow-end.png)
