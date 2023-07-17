---
audience: end-user
title: 使用「擴充」工作流程活動
description: 了解如何使用「擴充」工作流程活動
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '626'
ht-degree: 100%

---


# 擴充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="擴充活動"
>abstract="擴充活動可讓您使用資料庫中的其他資訊來增強目標資料。這通常會用於目標定位活動之後的工作流程。<br/>將擴充資料新增到工作流程後，它可以用於在擴充活動之後新增的活動中，根據客戶的行為、偏好和需求將客戶分成不同群組，或是用於建立最有可能讓目標對象產生共鳴的個人化行銷訊息和行銷活動。"

「**擴充**」活動是一種「**目標定位**」活動。此活動可讓您使用資料庫中的其他資訊來增強目標資料。這通常會用於分段活動之後的工作流程。

擴充資料可以：

* **來自相同工作表**，作為您工作流程中的目標：

  *以一組客戶為目標，並新增「生日」欄位到目前工作表*

* **來自另一個工作表**：

  *以一組客戶為目標，並新增來自「購買」表格的「數量」和「產品類型」欄位*。

將擴充資料新增到工作流程後，即可將其用於&#x200B;**擴充**&#x200B;活動之後新增的活動中，以根據客戶的行為、偏好和需求將客戶分成不同群組，或是用於建立最有可能讓目標對象產生共鳴的個人化行銷訊息和行銷活動。

例如，您可以將與客戶購買行為相關資訊新增到工作流程的工作表中，並使用此資料根據客戶上次購買行為或消費金額量身訂製電子郵件。

## 一般設定 {#general}

請按照以下步驟設定&#x200B;**擴充**&#x200B;活動：

1. 新增活動，例如「**建置對象**」和「**組合**」活動。
1. 新增「**擴充**」活動。
1. 按一下「**新增擴充資料**」。

![](../assets/workflow-enrichment1.png)

您可以選取兩種類型的擴充資料：來自目標維度的[單一擴充屬性](#single-attribute)，或是[集合連結](#collection-link)。

## 單一擴充屬性 {#single-attribute}

在這裡，我們只新增單一擴充屬性，例如出生日期。請按照以下步驟操作：

1. 按一下「**屬性**」欄位內部。
1. 在目標定位維度中選取一個簡單的欄位，在範例中是出生日期。
1. 按一下「**確認**」。

![](../assets/workflow-enrichment2.png)

## 集合連結 {#collection-link}

在這個較複雜的使用案例中，我們要選取集合連結，這是表格之間具有 1-N 基數的連結。讓我們擷取最近三筆低於 100 美元的購買。為了這麼做，您需要定義：

* 擴充屬性：「**總金額**」欄位
* 要擷取的行數：3
* 篩選：篩除大於 100 美元的項目
* 排序：「**訂購日期**」欄位的遞減排序。

### 新增此屬性

您可以在此處選取用作擴充資料的集合連結。

1. 按一下「**屬性**」欄位內部。
1. 按一下「**顯示進階屬性**」。
1. 選取「**總金額**」欄位 (在「**購買**」表格中)。

![](../assets/workflow-enrichment3.png)

### 定義集合設定

然後，定義收集資料的方式以及要擷取的記錄數。

1. 選取「**集合資料**」(從「**選取收集資料的方式**」下拉選單)。
1. 在「**要擷取的行 (要建立的欄)**」欄位輸入「3」。

![](../assets/workflow-enrichment4.png)

例如，如果您想要取得某個客戶的平均購買金額，請改為選取「**彙總資料**」，然後選取「**平均**」(從「**彙總函數**」下拉選單)。

![](../assets/workflow-enrichment5.png)

### 定義篩選條件

在這裡，我們可定義擴充屬性的最大值。我們會篩除大於 100 美元的項目。

1. 按一下「**編輯篩選條件**」。
1. 新增以下兩個篩選條件：「**總金額**&#x200B;存在」以及「**總金額**&#x200B;小於 100」。第一個會篩選出 NULL 值，因為這會顯示為最大值。
1. 按一下「**確認**」。

![](../assets/workflow-enrichment6.png)

### 定義排序

我們現在需要套用排序，以擷取三筆&#x200B;**最近的**&#x200B;購買。

1. 啟動「**啟用排序**」選項。
1. 按一下「**屬性**」欄位內部。
1. 選取「**訂購日期**」欄位。
1. 按一下「**確認**」。
1. 選取「**遞減**」(從「**排序**」下拉選單)。

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->