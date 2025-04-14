---
audience: end-user
title: 關於唯讀工作流程
description: 瞭解工作流程處於唯讀模式的原因
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 4%

---

# 關於唯讀工作流程 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="This workflow is read only"
>abstract="You cannot edit this workflow due to your rights or the type of the workflow."

Campaign使用者存取Adobe Campaign資料的能力可能受到限制。 Campaign管理員可以授予他們檢視特定功能的許可權，但不授予他們編輯或修改這些功能的許可權。 資料的使用者許可權是確保資料和流程安全性的基本要素。 在[本節](../get-started/permissions.md)中進一步瞭解Campaign的許可權管理。

當工作流程處於唯讀模式時：

* 提及&#x200B;**[!UICONTROL 唯讀]**&#x200B;出現在&#x200B;**[!UICONTROL 設定]**&#x200B;按鈕附近。
* 無法存取動作按鈕。

![唯讀工作流程介面，顯示設定按鈕和停用的動作按鈕。](assets/readonly-workflow.png){zoomable="yes"}

使用者無法在唯讀工作流程中編輯任何內容。 他們不可變更活動的設定。

![排程器介面處於唯讀模式，顯示已停用的設定選項。](assets/scheduler-readonly.png){zoomable="yes"}

使用者無法刪除工作流程。

![介面顯示刪除工作流程的限制許可權。](assets/readonly-rights.png){zoomable="yes"}

## 唯讀工作流程的型別 {#readonly-workflow-types}

視工作流程型別而定，唯讀模式可能會有所不同。

### 行銷活動工作流程 {#readonly-campaign-wf}

在唯讀行銷活動工作流程中，使用者無法存取監視按鈕。

![促銷活動工作流程介面處於唯讀模式，顯示停用的監視選項。](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 技術工作流程 {#readonly-tech-wf}

所有Campaign使用者（包括管理員）的內建技術工作流程均為唯讀。 不過，使用者可視需要&#x200B;**暫停**&#x200B;或&#x200B;**停止**。 僅允許這些動作。

![技術工作流程介面處於唯讀模式，顯示暫停或停止工作流程的選項。](assets/readonly-technical-workflow.png){zoomable="yes"}

在[本節](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)中進一步瞭解技術工作流程。