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
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945761"
---
# <a name="hide-public-folders"></a>ซ่อนโฟลเดอร์สาธารณะ

**เมื่อต้องการซ่อนทรีโฟลเดอร์สาธารณะทั้งหมด**:

ใช้ขั้นตอน [ในบทความนี้](https://aka.ms/ControlPF) เพื่อซ่อนทรีโฟลเดอร์สาธารณะทั้งหมดจากผู้ใช้ที่เลือกหรือผู้ใช้ทั้งหมด

**เมื่อต้องการซ่อนโฟลเดอร์สาธารณะที่ระบุ**:

1. เพิ่มสิทธิ์ของผู้ใช้ที่ต้องการเข้าถึงโฟลเดอร์สาธารณะ

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. เอาผู้ใช้ **ค่าเริ่มต้น** ออกจาก **รายการ** สิทธิ์:

    `Remove-PublicFolderClientPermission \test1 -User Default`
