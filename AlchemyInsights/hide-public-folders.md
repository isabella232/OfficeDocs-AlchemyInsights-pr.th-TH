---
title: ซ่อนโฟลเดอร์สาธารณะ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315442"
---
# <a name="hide-public-folders"></a>ซ่อนโฟลเดอร์สาธารณะ

**เมื่อต้องการซ่อนทรีโฟลเดอร์สาธารณะทั้งหมด**:

ใช้ [ขั้นตอนในบทความนี้เพื่อ](https://aka.ms/ControlPF) ซ่อนทรีโฟลเดอร์สาธารณะทั้งหมดจากผู้ใช้ที่เลือกหรือผู้ใช้ทั้งหมด

**เมื่อต้องการซ่อนโฟลเดอร์สาธารณะเฉพาะ:**

1. เพิ่มสิทธิ์ให้กับผู้ใช้ที่ต้องการเข้าถึงโฟลเดอร์สาธารณะ

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. เอาผู้ใช้ **เริ่มต้นจาก****รายการสิทธิ์**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
