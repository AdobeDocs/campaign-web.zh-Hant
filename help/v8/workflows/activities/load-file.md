---
audience: end-user
title: 使用載入檔案工作流程活動
description: 瞭解如何使用載入檔案工作流程活動
badge: label="有限可用性"
source-git-commit: 88daf84e617595a80c5cd3fd536969618f0fdcf5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 33%

---

# 載入檔案 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="載入檔案活動"
>abstract="此 **載入檔案** 活動是 **資料管理** 活動。 使用此活動來處理儲存在外部檔案中的資料。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="範例檔案"
>abstract="範例檔案"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="檔案名稱"
>abstract="檔案名稱"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Target 資料庫"
>abstract="Target 資料庫"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="拒絕載入檔案活動的管理"
>abstract="拒絕載入檔案活動的管理"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="拒絕管理傳出轉變"
>abstract="拒絕管理傳出轉變"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="拒絕管理拒絕的傳出轉變"
>abstract="拒絕管理拒絕的傳出轉變"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="載入檔案活動的格式化"
>abstract="載入檔案活動的格式化"


此 **載入檔案** 活動是 **資料管理** 活動。 使用此活動來處理儲存在外部檔案中的設定檔和資料。 設定檔和資料不會新增至資料庫，但輸入檔案中的所有欄位都可用於 [個人化](../../personalization/gs-personalization.md)，或更新設定檔或任何其他表格。


>[!NOTE]
>支援的檔案格式為：文字(TXT)和逗號分隔值(CSV)。


此活動可搭配 [調解](reconciliation.md) 活動，將未識別的資料連結至現有資源。 例如， **載入檔案** 活動可放置在 **調解** 活動（如果將非標準資料匯入資料庫）。


## 設定載入檔案活動 {#load-configuration}

請依照下列步驟設定 **載入檔案** 活動：


1. 拖放 **載入檔案** 活動放入工作流程。 按一下 **從檔案選取** 按鈕。
1. 選取要使用的本機檔案。 格式必須與此對齊 [範例檔案](../../audience/file-audience.md#sample-file).
1. 在畫面中央區段預覽並檢查資料的對應方式。
1. 調整欄設定以及從可用選項中格式化資料的方式。
1. 當設定正確時，按一下「**確認**」。

## 範例{#load-example}

外部檔案載入的範例可在 **調解** 中的活動 [本節](reconciliation.md#example).