---
audience: end-user
title: 使用AND聯結工作流程活動
description: 瞭解如何使用「與」結合工作流程活動
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 4%

---


# AND-join {#join}

此 **合併連結** 活動可讓您同步工作流程的多個執行分支。

AND-join活動只會在所有入站轉變啟動後，才會觸發其出站轉變，換句話說，會在所有先前活動完成後觸發。

請依照下列步驟設定 **合併連結** 活動：

1. 新增多個活動，例如 **合併** 至少形成兩個不同執行分支的活動。
1. 新增 **合併連結** 活動至任何分支。
1. 在 **合併選項** 區段，勾選所有您欲加入的先前活動。
1. 選取 **主要集** 要保留在出站轉變中。
