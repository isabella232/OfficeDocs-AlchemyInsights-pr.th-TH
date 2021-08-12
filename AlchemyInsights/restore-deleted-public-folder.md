---
title: คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943394"
---
# <a name="restore-a-deleted-public-folder"></a>คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ

**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:

- ให้ดูที่[คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook 2016](https://aka.ms/pfrec)ได้
 
**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดๆ)**: 

- โปรดใช้การสั่ง EXO PowerShell ต่อไปนี้:

    ไวยากรณ์:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    ตัวอย่าง: The following command will restore Subfolder1 and place it under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ดูรายละเอียด [เพิ่มเติมที่ คืนค่าโฟลเดอร์](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) สาธารณะที่ถูกลบ
