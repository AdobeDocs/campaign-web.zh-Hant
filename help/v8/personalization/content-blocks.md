---
title: 在 Campaign 中個人化您的內容
description: 了解如何在 Adobe Campaign Web UI 中個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: ht
source-wordcount: '277'
ht-degree: 100%

---


# 內建的內容區塊 {#ootb-content-blocks}

內建的內容區塊包括：

* **[!UICONTROL 由 Adobe Campaign 啟用]**：插入「由 Adobe Campaign 啟用」標誌。
* **[!UICONTROL 專有名詞的格式化函數]**：產生 **[!UICONTROL toSmartCase]** Javascript 函數，它將每個單詞的第一個字母變更為大寫。
* **[!UICONTROL 問候語]**：插入帶有收件人全名的問候語，後面跟著一個逗號。範例：「你好 John Doe，」。
* **[!UICONTROL 插入標誌]**：插入在執行個體中定義的標誌。
* **[!UICONTROL 鏡像頁面連結]**：插入[鏡像頁面](../content/mirror-page.md)的連結。預設格式：「如果您無法正確檢視此訊息，請按一下此處」。
* **[!UICONTROL 鏡像頁面 URL]**：插入鏡像頁面 URL，使傳遞設計工具檢查連結。
* **[!UICONTROL 單一模式的優惠接受 URL]**：插入可以將優惠設定為&#x200B;**[!UICONTROL 接受]** 的 URL。(如果啟用互動模組，則此區塊可用)
* **[!UICONTROL 註冊確認]**：插入可以確認訂閱的連結。
* **[!UICONTROL 註冊連結]**：插入訂閱連結。此連結在執行個體設定中定義。預設內容：「若要註冊，請按一下這裡。」
* **[!UICONTROL 註冊連結 (含推薦者)]**：插入可以識別訪客和傳遞的訂閱連結。此連結在執行個體設定中定義。
* **[!UICONTROL 註冊頁面 URL]**：插入訂閱 URL
* **[!UICONTROL 內容電子郵件的樣式]**&#x200B;和&#x200B;**[!UICONTROL 通知樣式]**：產生使用預先定義的 HTML 樣式格式化電子郵件的程式碼。
* **[!UICONTROL 取消訂閱連結]**：插入可以取消訂閱所有傳遞 (封鎖清單) 的連結。預設關聯內容：「您收到此訊息因為您曾聯絡&#x200B;***您的組織名稱***&#x200B;或附屬機構。若不要再收到來自&#x200B;***您的組織名稱***&#x200B;的訊息，請按一下這裡。」
