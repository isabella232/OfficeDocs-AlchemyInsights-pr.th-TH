---
title: การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774550"
---
# <a name="restore-a-deleted-public-folder"></a>การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ

**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะให้ใช้วิธีต่อไป**นี้

- ให้ดู[ที่คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่อีเมลใน Outlook ๒๐๑๖](https://aka.ms/pfrec)
 
**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ตาม)**: 

- โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:

    ไวยากรณ์ของ

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ให้ดู [ที่คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) สำหรับรายละเอียดเพิ่มเติม
