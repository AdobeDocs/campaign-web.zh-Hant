---
audience: end-user
title: 關於唯讀工作流程
description: 瞭解工作流程處於唯讀模式的原因
source-git-commit: 6985e8cb11f12ab7818cc71441a4d3b41f1a0493
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# 關於唯讀工作流程 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="此工作流程為唯讀資料"
>abstract="由於您的許可權或工作流程的型別，您無法編輯此工作流程。"

某些工作流程可能處於唯讀模式。 您可以透過以下方式檢視：

- 提及內容 **[!UICONTROL **&#x200B;唯讀&#x200B;**]**  在 **[!UICONTROL 設定]** 按鈕
- 無法存取動作按鈕

![](assets/readonly-workflow.png){zoomable="yes"}

您無法編輯唯讀工作流程中的任何專案。 您不可變更活動的設定。


![](assets/scheduler-readonly.png){zoomable="yes"}


您也無權刪除工作流程。

![](assets/readonly-rights.png){zoomable="yes"}

## 為何唯讀工作流程

唯讀模式適用於沒有許可權和存取許可權的使用者，可編輯這些工作流程。 [在此處瞭解更多](../get-started/permissions.md)

行銷活動使用者對於可在Adobe Campaign中存取的資料可能有限制。 管理員可讓他檢視部分功能，但無法加以處理。

## 唯讀工作流程的型別

根據工作流程的型別，唯讀模式可能會有所不同。

### 行銷活動工作流程

在唯讀行銷活動工作流程的情況下，使用者無法存取監視按鈕。

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 技術工作流程

行銷活動使用者的技術工作流程處於唯讀模式。
內建的技術工作流程對所有人而言都是唯讀模式，即使是管理員使用者亦然。 但使用者可以 **pause** 或 **停止** 視需要提供。 僅允許這些動作。 [在此處瞭解更多](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}