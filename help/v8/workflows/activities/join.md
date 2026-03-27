---
audience: end-user
title: 使用加入工作流程活動
description: 瞭解如何使用加入工作流程活動
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 20%

---

# 加入 {#join}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="多個工作流程分支和加入活動"
>abstract="現在支援多個分支。 您可以按一下工具列上的「新增分支」 ，而不使用「分支」 。 合併連結活動也已改善。 它現在是通用的「聯結」活動，可讓您在「與」和「或」聯結選項之間選擇。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hant" text="請參閱發行說明"

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="合併連結活動"
>abstract="**合併連結**&#x200B;活動可讓您同步處理工作流程的多個執行分支。一旦所有前面的活動完成，就會觸發此活動。這樣能確保特定活動已完成後再繼續執行工作流程。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="連接活動"
>abstract="**加入**&#x200B;活動可讓您合併多個入站轉變。 選擇在所有入站轉變完成(AND)時還是任何入站轉變完成(OR)時繼續。"

**加入**&#x200B;活動是&#x200B;**流量控制**活動。 它會同步工作流程的多個執行分支。
您可以選擇如何評估入站轉變：

* **AND**：僅在啟動所有選取的入站轉變後繼續。
* **OR**：在啟動一個選取的入站轉變後立即繼續。

選取&#x200B;**AND**&#x200B;時，此活動只有在啟動所有入站轉變之後，才會觸發其出站轉變。 換言之，它會在所有先前的活動完成後啟動。 這可確保在繼續執行工作流程之前已完成某些活動。

選取&#x200B;**或**&#x200B;時，只要其中一個選取的入站轉變啟動，就會繼續執行。 不會等待每個分支。

## 設定加入活動 {#join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="合併選項"
>abstract="選取您要參加的活動。在「**主要集合**」下拉選單中，選擇您要保留的傳入轉變群體。"

請依照下列步驟設定&#x200B;**加入**&#x200B;活動：

1. 新增多個活動（例如管道活動）以形成至少兩個不同的執行分支。 您可以使用&#x200B;**分支**，或使用&#x200B;**新增分支** (+)工具列按鈕新增個別的分支。 請參閱[協調活動](../orchestrate-activities.md#toolbar)。

   ![熒幕擷圖顯示兩個分支。](../assets/workflow-join.png)

1. 將&#x200B;**加入**&#x200B;活動新增至任何分支。

   ![熒幕擷圖顯示新增的加入活動。](../assets/workflow-join2.png)

1. 在加入選項中，選擇&#x200B;**AND**&#x200B;或&#x200B;**OR**，然後按一下&#x200B;**繼續**。
1. 在&#x200B;**合併選項**&#x200B;區段中，勾選所有先前要加入的活動。
1. 在&#x200B;**主要集**&#x200B;下拉式清單中，選擇要保留的入站轉變母體。 傳出轉變只能包含其中一個傳入轉變群體。

   >[!NOTE]
   >
   >**主要集**&#x200B;欄位僅適用於&#x200B;**AND**&#x200B;加入選項。

   ![顯示已設定加入的熒幕擷圖。](../assets/workflow-join3.png)

## 範例 {#join-example}

以下範例顯示兩個工作流程分支，各包含電子郵件和簡訊傳遞。啟用兩個入站轉變時，會觸發設定為&#x200B;**AND**&#x200B;的&#x200B;**加入**&#x200B;活動。 推播通知只會在兩個傳送完成後傳送。 如果您將加入選項設為&#x200B;**或**，則當第一個傳入傳遞活動完成時，就會立即傳送推送訊息。

![具有兩個分支的工作流程範例，顯示電子郵件和SMS傳遞後接推播通知。](../assets/workflow-join4.png){zoomable="yes"}