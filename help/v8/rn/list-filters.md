---
audience: end-user
title: Campaign Web v8的新增功能
description: 探索Campaign Web v8的新功能
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: 9f9cb4423d098ae57f429fb2a49e335d413399c1
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 65%

---


# 新增功能? {#new}

## Alpha 2.0版{#alpha-release}

這個新的 Campaign Web 介面目前僅提供給 **Alpha 實作者**，具有以下功能：

**現代、直覺和統一的體驗**

新的 Campaign Web UI 提供全新的使用者體驗，與所有 Adobe Experience Cloud 解決方案和應用程式保持一致。它提供以下功能：

* 透過單一和共用使用者工作階段存取新介面以及您的其他Adobe解決方案
* 新的導覽體驗，左側邊欄提供所有選單和資料夾
* 頂端列中的解決方案和組織切換器
* 與 Unified Shell 整合，可直接存取社群、說明中心和支援

**全新強大的功能及順暢的流程**

* 重新想像的工作流程畫布介面以設計和管理您的流程
* 動態內容，可為您的對象提供極具針對性和個人化的體驗
* 與Adobe Experience Platform受眾的原生整合
* 工作流程、傳遞、行銷活動和內容的範本管理

在[此頁面](../get-started/user-interface.md)進一步了解新的 UI。

**建立、啟動和測量您的行銷活動**

使用新的 Campaign Web UI 可以：

* 使用電子郵件設計工具設計個人化的電子郵件內容 - [了解更多](../content/edit-content.md)
* 傳送跨管道行銷活動，包括簡訊和推播通知。
* 使用規則產生器定義目標對象 - [了解更多](../audience/about-audiences.md)
* 預覽、測試和傳送您的電子郵件訊息 - [了解更多](../monitor/prepare-send.md)
* 使用內建的報告監控、傳送和測量結果 - [了解更多](../reporting/delivery-reports.md)


## 轉換至Campaign Web UI

身為Campaign使用者，您仍然可以存取使用者端主控台，以建置和管理Campaign資源和元件。 資料和設定會從一個環境同步到另一個環境。 在[本章節](../get-started/get-started.md#about-campaign-client-consoleac-client)了解更多資訊。

此外，從Explorer左側導覽中，使用者端主控台中可用的所有資料和設定都會顯示在Campaign Web UI中。 進一步瞭解中的總管檢視 [本節](../get-started/user-interface.md#explorer-user-interface-explorer).


## 術語更新 {#terminology-updates}

您身為現有 Campaign 使用者，請注意一些概念已重新命名以符合最新的術語標準。這些變更僅適用於 Campaign Web UI，不會反映在用戶端主控台。它們總結如下。

* 校訂現在是&#x200B;**測試電子郵件**：若要傳送校訂，請使用電子郵件傳遞 UI 中的「**測試**」按鈕。校訂目標的目標現在稱為&#x200B;**測試設定檔**
* 種子地址現在是&#x200B;**測試設定檔**：傳送測試電子郵件到種子地址，這些地址是資料庫中額外和虛構的收件者
* 傳遞分析現在是&#x200B;**傳遞準備**。當您需要啟動分析時，按一下「**準備**」按鈕
* 電子郵件預覽現在透過「**模擬內容**」按鈕提供
* 清單現在是&#x200B;**對象**

## 限制{#limitations-alpha}

此 Alpha 版本有以下限制：

* 唯一可編輯的物件是傳送、行銷活動、工作流程、對象和範本。 其他物件是唯讀的。使用篩選器來瀏覽全部物件。
* 無法儲存對象以供日後使用。
* 尚未提供管理使用者介面。
* 報告量度 (例如開啟和追蹤資料) 每小時更新一次。
* 傳遞儀表板 KPIs 每 5 分鐘更新一次。- 但傳遞準備是即時的。
* 尚未整合頂端列中的 Adobe Experience Cloud 通知和統一說明。

