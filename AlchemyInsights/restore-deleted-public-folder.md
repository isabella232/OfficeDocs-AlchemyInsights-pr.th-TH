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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063766"
---
# <a name="restore-a-deleted-public-folder"></a>การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ

**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:

- ดู[คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook ๒๐๑๖](https://aka.ms/pfrec)
 
**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ได้)**: 

- โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:

    ไวยากรณ์:

    >$pf = ได้รับ PublicFolder \ NON_IPM_SUBTREE DUMPSTER_ROOT-Recurse |? {$_. ชื่อ-eq "\<name_of_deleted_public_Folder"}; $Pf ตั้งค่า PublicFolder- \<เส้นทางเส้นทางที่จะคืนค่าโฟลเดอร์>

    ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:

    >$pf = ได้รับ PublicFolder \ NON_IPM_SUBTREE DUMPSTER_ROOT-Recurse |? {$_. ชื่อ-eq "Subfolder1"}; $Pf ตั้งค่า PublicFolder-เส้นทาง \Parent1

ดู[ที่การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)สำหรับรายละเอียดเพิ่มเติม
