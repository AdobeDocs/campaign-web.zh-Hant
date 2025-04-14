---
title: 目標市場選擇維度
description: 進一步瞭解Adobe Campaign網頁中的目標維度功能
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 11%

---

# 目標市場選擇維度 {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="選取目標市場選擇維度"
>abstract="目標維度可讓您定義作業的目標母體：收件者、合約受益者、操作者、訂閱者等。 對於電子郵件和簡訊，依預設，目標是從收件者內建表格中選取。對於推播通知，預設目標市場選擇維度是訂閱者應用程式。"

目標維度（也稱為目標對應）是作業處理的資料型別。 它定義目標母體，例如設定檔、合約受益人、運運算元或訂閱者。

## 工作流程的目標維度 {#workflow}

工作流程的目標維度是由第一個&#x200B;**[!UICONTROL 建立對象]**&#x200B;活動所定義，並用於所有後續活動，直到工作流程結束為止。 例如，從資料庫查詢設定檔時，出站轉變包含「recipient」型別的資料，這會傳輸到下一個活動。

使用[變更維度活動](../workflows/activities/change-dimension.md)在工作流程中切換目標維度。 這可查詢特定表格（例如購買或訂閱）上的資料庫，然後變更收件者的目標維度，以將傳送內容傳送至對應的設定檔。

選取目標維度時（在工作流程設定中或在&#x200B;**建立對象**、**調解**&#x200B;或&#x200B;**變更維度**&#x200B;等活動中），預設會顯示常用結構描述清單。 若要顯示所有可用的結構描述，請切換&#x200B;**[!UICONTROL 顯示所有結構描述]**&#x200B;按鈕。 系統會為每個使用者儲存選項選取範圍。

![熒幕擷圖顯示目標維度介面，並啟用[顯示所有結構描述]按鈕。](assets/targeting-dimension-show-all.png){zoomable="yes"}

## 目標市場選擇維度 {#list}

依預設，電子郵件和簡訊傳遞範本會定位設定檔。 他們的目標維度使用&#x200B;**nms：recipient**&#x200B;資料表的欄位。 對於推播通知，預設目標維度為連結至收件者表格的&#x200B;**訂閱者應用程式nms：appSubscriptionRcp**。

在工作流程與傳遞中使用其他內建的目標對應，如下所列：

| 名稱 | 使用傳送至 | 結構描述 |
|-----------------------|-------------------------------------------------------|-------------------------|
| 收件者 | 設定檔/收件者（內建收件者表格） | nms：recipient |
| 訪客 | 透過反向連結收集設定檔的訪客（例如病毒式行銷） | mns：visitor |
| 訂閱 | 訂閱新聞稿等資訊服務的設定檔 | nms：subscription |
| 訪客訂閱 | 訂閱資訊服務的訪客 | nms：visitorSub |
| 運算子 | Adobe Campaign運運算元 | nms：operator |
| 外部檔案 | 透過包含所有必要資訊的檔案傳遞 | 沒有連結的結構描述，沒有輸入目標 |
| 訂閱者應用程式 | 訂閱應用程式的設定檔 | nms：appSubscriptionRcp |

此外，根據特定需求建立新的目標對應。 僅從使用者端主控台執行此作業。 深入瞭解[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}。