---
audience: end-user
title: Campaign Web v8發行說明
description: Campaign Web v8發行說明
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Infertitive"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# 發行說明 {#release-notes}

本頁列出Campaign Web v8的所有最新功能和改進項目。

## Alpha版{#alpha-release}

這個新的Campaign網頁介面目前僅適用於 **Alpha練習者** 功能：

**現代、直覺且統一的體驗**

Campaign新的Web UI提供與所有Adobe Experience Cloud解決方案和應用程式一致的新使用者體驗。 它提供：

* 透過單一和共用的使用者工作階段存取新介面和其他Adobe解決方案
* 新的導覽體驗，所有功能表和資料夾皆可從左側邊欄取得
* 從頂端列切換解決方案和組織
* 統一殼層整合，可直接存取社群、說明中心和支援
<!--
No search and pulse notifications in Alpha
-->

深入了解新UI，請參閱 [本頁](../get-started/user-interface.md).

**建立、啟動和測量您的電子郵件行銷活動**

使用新的Campaign網頁UI來：

* 使用電子郵件設計工具設計個人化電子郵件內容 —  [深入了解](../content/edit-content.md)
* 使用規則產生器定義目標對象 —  [深入了解](../audience/about-audiences.md)
* 預覽、測試和傳送您的電子郵件訊息 —  [深入了解](../monitor/prepare-send.md)
* 使用內建報告監視傳送和測量結果 —  [深入了解](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## 術語更新{#terminology-updates}

請注意，作為現有的Campaign使用者，有些概念已重新命名以符合最新的術語標準。 這些變更只會套用至Campaign Web UI，不會反映在用戶端主控台中。 以下概述。

* 現在提供校樣 **測試電子郵件**:若要傳送校樣，請使用 **測試** 按鈕。 校樣目標的目標現在稱為 **測試設定檔**
* 種子地址現在用作 **測試設定檔**:將測試電子郵件傳送至種子地址，這些地址是資料庫中其他虛構的收件者
* 傳遞分析現在是 **傳遞準備**. 當您需要啟動分析時，按一下 **準備** 按鈕
* 現在可透過 **模擬內容** 按鈕
* 清單現在 **對象**

## 限制{#limitations-alpha}

測試版將提供某些Campaign重要功能，例如跨通道行銷活動和工作流程管理。

以下限制適用於此Alpha版：

* 唯一可編輯的對象是「傳送」。 其他則是唯讀的。 使用篩選器來瀏覽所有項目。
* 此版本是專為一次電子郵件行銷活動而設計。 尚不支援其他管道。
* 管理用戶介面不可用。
* 報告量度（例如開啟和追蹤資料）每小時更新一次。
* 傳送控制面板KPI每5分鐘更新一次。  — 但傳送準備是即時的。
* 頂端列中提供的Adobe Experience Cloud通知和統一說明尚未整合。

