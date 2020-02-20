---
title: การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158546"
---
# <a name="restore-a-deleted-public-folder"></a>การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ

**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:

- ดู[คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook ๒๐๑๖](https://aka.ms/pfrec)
 
**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ได้)**: 

- โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:

    ไวยากรณ์:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ดู[ที่การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)สำหรับรายละเอียดเพิ่มเติม
