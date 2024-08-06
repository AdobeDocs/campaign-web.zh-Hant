---
audience: end-user
title: Campaign Web 使用者介面中的權限管理
description: 深入了解 Campaign Web 使用者介面的權限
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: ht
source-wordcount: '228'
ht-degree: 100%

---


# 權限 {#permissions}

Adobe Campaign 中的每位使用者在應用程式中都有其權限和限制。使用者可以是操作者群組的一員，並繼承該群組的權限。

根據其權限，操作者可以：

* 存取特定功能
* 存取特定資料
* 存取特定動作 (建立、修改、刪除)

若要了解在 Adobe Campaign 中設定權限的詳細程序，請參閱 [Adobe Campaign v8 (控制台) 文件](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}。

## 資料夾權限 {#folder-permissions}

根據您的權限，您可以在「**[!UICONTROL 資料夾設定]**」中檢視和管理資料夾權限。

以下是傳遞資料夾的範例：

![](assets/folder_settings.png){zoomable="yes"}

在「**[!UICONTROL 資料夾設定]**」的「**[!UICONTROL 安全性]**」區段中，您可以檢視和管理 (新增或刪除) 可存取該資料夾的操作者或群組。

![](assets/folder_security.png){zoomable="yes"}

您可以直接按一下該權限，並將其變更為「**[!UICONTROL 已允許]**」或「**[!UICONTROL 已拒絕]**」。

![](assets/folder_security_denied.png){zoomable="yes"}

如果啟用「**[!UICONTROL 傳播]**」選項，針對資料夾定義的所有權限都會套用至其所有的子資料夾。每個子資料夾都可以過載這些權限。

如果勾選了「**[!UICONTROL 系統資料夾]**」選項，則所有操作者都可以存取 (無論其權限為何)。

您也可以[在 Adobe Campaign 控制台中管理資料夾權限](https://experienceleague.adobe.com/zh-hant/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}。

Campaign Web 使用者介面中的所有權限都會與 Campaign 用戶端控制台權限進行同步。
