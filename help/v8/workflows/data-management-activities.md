---
audience: end-user
title: 使用工作流程資料管理活動
description: 了解如何將資料管理活動用於Adobe Campaign網頁工作流程
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 1%

---

# 資料管理活動 {#data-management}

概述：它們的用途，您可以對它們執行哪些使用案例

列出可用活動+簡短說明+區段參考

## 擴充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="擴充活動"
>abstract="「擴充」活動可讓您使用資料庫的其他資訊增強目標資料。 它通常用於目標定位活動後的工作流程中。<br/>擴充資料新增至工作流程後，便可用於擴充活動後新增的活動，以根據客戶的行為、偏好和需求，將客戶細分為不同的群組，或建立更可能與目標對象產生迴響的個人化行銷訊息和行銷活動。"

「擴充」活動可讓您使用資料庫的其他資訊增強目標資料。 它通常用於目標定位活動後的工作流程中。

擴充資料可能會出現：

* **從同一工作表** 作為目標進入工作流程的對象：

   *定位一組客戶，並將「出生日期」欄位添加到當前工作表*

* **從另一個工作表**:

   *定位一組客戶，並新增「購買」表格中的「金額」和「產品類型」欄位*.

擴充資料新增至工作流程後，便可用於擴充活動後新增的活動，以根據客戶的行為、偏好和需求，將客戶細分為不同的群組，或建立更可能與目標對象產生迴響的個人化行銷訊息和行銷活動。

例如，您可以將與客戶購買相關的工作表資訊新增至工作流程，並使用此資料以客戶的最新購買或這些購買所花費的金額來個人化電子郵件。

若要將Enricment活動新增至您的工作流程，請執行下列步驟：

1. 新增活動
1. 選取屬性作為擴充資料

   顯示高級欄位選項i按鈕

   注意：目標維度的屬性

1. 選取資料的收集方式
1. 如果要檢索多個記錄的集合，則要檢索的記錄數
1. 套用篩選器和建置規則

   選擇現有篩選器保存篩選器，以便以可視方式或在代碼視圖中重新使用篩選器的視圖結果

1. 使用屬性對記錄進行排序

利用行銷活動中的擴充資料

我們可以在其中使用擴充資料：個人化電子郵件，其他使用案例？