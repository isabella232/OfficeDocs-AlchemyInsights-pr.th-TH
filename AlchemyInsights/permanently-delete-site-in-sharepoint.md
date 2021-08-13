---
title: ลบไซต์อย่างถาวรในSharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944330"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>ลบไซต์อย่างถาวรในSharePoint

เมื่อต้องการใช้ URL จากไซต์ที่ถูกลบ (เพื่อสร้างไซต์ใหม่) หรือเมื่อต้องการลบไซต์อย่างถาวรเนื่องจากไซต์ดังกล่าวไม่ได้ใช้อยู่อีกต่อไป คุณสามารถใช้ ลบถาวร จากศูนย์การจัดการ SharePointใหม่ ได้ 

1. ไปที่หน้า[ไซต์ที่ถูกลบ ของศูนย์SharePointและ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)ลงชื่อเข้าใช้ด้วยบัญชีที่มีสิทธิ์ผู้ดูแลระบบขององค์กรของคุณ 

2. ในคอลัมน์ด้านซ้าย ให้เลือกไซต์ 

3. **คลิก ลบ** ถาวร 

**หมายเหตุ**: ไซต์ที่เชื่อมต่อกับกลุ่มไม่สามารถถูกลบออกจากศูนย์การจัดการSharePointใหม่ได้อย่างถาวร [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.  

For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
