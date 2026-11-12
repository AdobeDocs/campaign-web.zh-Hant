---
title: 轉換至Campaign v8後的檢查及疑難排解
description: 瞭解從Campaign Standard轉換至Campaign v8後，要檢查哪些專案以及如何修正常見問題
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%
---
# 轉換後的檢查及疑難排解 {#post-transition-checks}

從Campaign Standard轉變為Campaign v8後，某些傳送、工作流程和登入頁面的行為可能與您的預期不同。 下表列出已轉換使用者報告的症狀、原因和做法。 如需完整的差異清單，請參閱[Campaign Standard與Campaign v8](acs-v8-differences.md)之間的差異。

| 症狀 | 原因和做法 | 了解更多 |
|---|---|---|
| 傳遞中的連結是直接URL，不會收集任何點按資料。 | 已在傳遞或它所依據的傳遞範本上停用追蹤。 檢查是否已啟用&#x200B;**啟用追蹤**，尤其是循環傳遞的範本。 | [追蹤設定](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| 透過「mailto」清單 — 取消訂閱方法取消訂閱的收件者不在隔離中。 | 這是預期中的情形。 這些收件者不會被傳送至隔離區。 他們將會從與傳送相關聯的服務中取消訂閱，或者如果傳送沒有服務，則新增到封鎖清單中。 若要追蹤這些取消訂閱，請檢查服務的訂閱或設定檔的&#x200B;**不再連絡**&#x200B;區段。 | [隔離](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| 登入頁面不會儲存由指令碼計算或儲存在隱藏欄位中的值。 | 在Campaign網頁使用者介面中建立的登入頁面不支援隱藏的輸入欄位或自訂JavaScript。 改為在使用者端主控台中將表單建立為網頁應用程式。 | [登陸頁面](../../v8/landing-pages/get-started-lp.md) |
| **檔案傳輸**&#x200B;找不到直接郵件活動產生的檔案。 | 直接郵件活動的出站轉變攜帶目標母體，而非擷取檔案。 加入&#x200B;**資料擷取**&#x200B;活動，然後加入&#x200B;**檔案傳輸**&#x200B;活動。 | [直接郵件](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| 多個傳遞批次會一起傳送。 | 從傳遞的聯絡日期開始排程波段。 如果傳送在某些波次的計畫時間後開始，這些波次會一起傳送，而不是彼此隔開。 | [使用波段傳送](../../v8/advanced-settings/send-using-waves.md) |
| 星號後有字元的檔案遮罩在Azure Blob儲存空間中找不到檔案。 | Azure Blob儲存體會依名稱前置詞來篩選檔案。 僅支援結尾星號。 | [轉移外部帳戶](../../v8/administration/transfer-external-account.md) |
| 在轉變之前傳送的傳遞映象頁面未開啟。 | 轉換前從Campaign Standard傳送的傳送映象頁面無法使用，且沒有因應措施。 從Campaign v8傳送的傳送映象頁面如常運作。 | [映象頁面](../../v8/email/mirror-page.md) |
| 使用自訂JavaScript的登陸頁面或內容區塊的行為方式不同。 | 自訂JavaScript在移轉期間會進行轉換，但會進行驗證和調整，尤其是當它使用`queryDef`、Campaign JavaScript API、工作階段寫入、組織單位處理或自訂URL產生時。 | [登陸頁面](../../v8/landing-pages/get-started-lp.md) |
