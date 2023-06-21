---
audience: end-user
title: Campaign Web v8 有哪些新增功能？
description: 探索 Campaign Web v8 附帶的新增功能
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha"
source-git-commit: 4a439abca9c7b1f2cc5d82214efb0aae033a996c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 97%

---


# 新增功能？ {#new}

## Alpha 2.0 版{#alpha-release}

這個新的 Campaign Web 介面目前僅提供給 **Alpha 實作者**，具有以下功能：

**現代、直覺和統一的體驗**

新的 Campaign Web UI 提供全新的使用者體驗，與所有 Adobe Experience Cloud 解決方案和應用程式保持一致。它提供以下功能：

* 使用單一和共用的使用者工作階段存取新介面和您的其他 Adobe 解決方案
* 新的導覽體驗，左側邊欄提供所有選單和資料夾
* 頂端列中的解決方案和組織切換器
* 與 Unified Shell 整合，可直接存取社群、說明中心和支援

**全新的強大功能和順暢無礙的流程**

* 重新想像的工作流程畫布介面，以用於設計和管理您的流程
* 動態內容可為您的對象提供目標明確的個人化體驗
* 和 Adob&#x200B;&#x200B;e Experience Platform 對象的原生整合
* 工作流程、傳遞、行銷活動和內容的範本管理

若要了解新 UI 的詳細資訊，請參閱[本頁面](../get-started/user-interface.md)。

**建立、啟動和測量您的行銷活動**

使用新的 Campaign Web UI 可以：

* 使用電子郵件設計工具設計個人化的電子郵件內容 - [了解更多](../content/edit-content.md)
* 傳送跨管道的行銷活動，包括簡訊和推播通知。
* 使用規則產生器定義目標對象 - [了解更多](../audience/about-audiences.md)
* 預覽、測試和傳送您的電子郵件訊息 - [了解更多](../monitor/prepare-send.md)
* 使用內建的報告監控、傳送和測量結果 - [了解更多](../reporting/delivery-reports.md)


## 轉換到 Campaign Web UI

由於您是 Campaign 使用者，因此仍然可以存取用戶端主控台，以建置和管理 Campaign 的資源與元件。資料和設定則會從一個環境同步至另一個環境。若要了解詳細資訊，請參閱[本章節](../get-started/get-started.md#about-campaign-client-consoleac-client)。

此外，您在用戶端主控台中已經可以使用的所有資料和設定都會從總管左側導覽顯示在 Campaign Web UI 中。若要了解總管檢視的詳細資訊，請參閱[本章節](../get-started/user-interface.md#explorer-user-interface-explorer)。


## 術語更新 {#terminology-updates}

您身為現有 Campaign 使用者，請注意一些概念已重新命名以符合最新的術語標準。這些變更僅適用於 Campaign Web UI，不會反映在用戶端主控台。它們總結如下。

* 校訂現在是&#x200B;**測試電子郵件**：若要傳送校訂，請使用電子郵件傳遞 UI 中的「**測試**」按鈕。校樣的目標現在稱為 **測試設定檔**. [了解更多](../preview-test/test-deliveries.md)。
* 種子地址現在是&#x200B;**測試設定檔**：傳送測試電子郵件到種子地址，這些地址是資料庫中額外和虛構的收件者.
* 傳遞分析現在是&#x200B;**傳遞準備**。當您需要啟動分析時，按一下「**準備**」按鈕。
* 電子郵件預覽現在會透過「**模擬內容**」按鈕提供.
* 清單現在是&#x200B;**對象**。

## 限制{#limitations-alpha}

此 Alpha 版本有以下限制：

* 唯一可編輯的物件是傳遞、行銷活動、工作流程、對象和範本。其他物件是唯讀的。使用篩選器來瀏覽全部物件。
* 無法將對象儲存以供未來使用。
* 尚未提供管理使用者介面。
* 報告量度 (例如開啟和追蹤資料) 每小時更新一次。
* 傳遞儀表板 KPIs 每 5 分鐘更新一次。- 但傳遞準備是即時的。
* 尚未整合頂端列中的 Adobe Experience Cloud 通知和統一說明。

