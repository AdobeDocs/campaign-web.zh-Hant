---
audience: end-user
title: Campaign Web v8 發行說明
description: Campaign Web v8 發行說明
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 100%

---


# 發行說明 {#release-notes}

此頁面列出 Campaign Web v8 的所有最新功能和改進項目。

## Alpha 版本{#alpha-release}

這個新的 Campaign Web 介面目前僅提供給 **Alpha 實作者**，具有以下功能：

**現代、直覺和統一的體驗**

新的 Campaign Web UI 提供全新的使用者體驗，與所有 Adobe Experience Cloud 解決方案和應用程式保持一致。它提供以下功能：

* 使用單一和共用的使用者工作階段，存取新介面和其他 Adobe 解決方案
* 新的導覽體驗，左側邊欄提供所有選單和資料夾
* 頂端列中的解決方案和組織切換器
* 與 Unified Shell 整合，可直接存取社群、說明中心和支援
<!--
No search and pulse notifications in Alpha
-->

在[此頁面](../get-started/user-interface.md)進一步了解新的 UI。

**建立、啟動和測量您的電子郵件行銷活動**

使用新的 Campaign Web UI 可以：

* 使用電子郵件設計工具設計個人化的電子郵件內容 - [了解更多](../content/edit-content.md)
* 使用規則產生器定義目標對象 - [了解更多](../audience/about-audiences.md)
* 預覽、測試和傳送您的電子郵件訊息 - [了解更多](../monitor/prepare-send.md)
* 使用內建的報告監控、傳送和測量結果 - [了解更多](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## 術語更新{#terminology-updates}

您身為現有 Campaign 使用者，請注意一些概念已重新命名以符合最新的術語標準。這些變更僅適用於 Campaign Web UI，不會反映在用戶端主控台。它們總結如下。

* 校訂現在是&#x200B;**測試電子郵件**：若要傳送校訂，請使用電子郵件傳遞 UI 中的「**測試**」按鈕。校訂目標的目標現在稱為&#x200B;**測試設定檔**
* 種子地址現在是&#x200B;**測試設定檔**：傳送測試電子郵件到種子地址，這些地址是資料庫中額外和虛構的收件者
* 傳遞分析現在是&#x200B;**傳遞準備**。當您需要啟動分析時，按一下「**準備**」按鈕
* 電子郵件預覽現在透過「**模擬內容**」按鈕提供
* 清單現在是&#x200B;**對象**

## 限制{#limitations-alpha}

一些 Campaign 關鍵功能，例如跨管道行銷活動和工作流程管理將在 Beta 版本提供。

此 Alpha 版本有以下限制：

* 唯一可編輯的物件是傳遞。其他物件是唯讀的。使用篩選器來瀏覽全部物件。
* 此版本專為一次性電子郵件行銷活動所設計。尚未支援其他管道。
* 尚未提供管理使用者介面。
* 報告量度 (例如開啟和追蹤資料) 每小時更新一次。
* 傳遞儀表板 KPIs 每 5 分鐘更新一次。- 但傳遞準備是即時的。
* 尚未整合頂端列中的 Adobe Experience Cloud 通知和統一說明。

