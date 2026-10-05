---
audience: end-user
title: 使用「結束工作流程」活動
description: 瞭解如何使用結束工作流程活動
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 54%
---
# 結束 {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="結束活動"
>abstract="「**結束**」活動可讓您以圖形方式標記工作流程的終點。 當存在多個傳入轉變時，請使用「**要連接的集合**」區段來選擇要連接到該活動的轉變。"

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
