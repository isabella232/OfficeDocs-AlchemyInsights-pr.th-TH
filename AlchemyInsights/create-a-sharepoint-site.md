---
title: การสร้างไซต์ SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786584"
---
# <a name="create-a-sharepoint-site"></a>การสร้างไซต์ SharePoint

สร้างหรือจัดการไซต์จาก [ไซต์ที่ใช้งานอยู่](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ในศูนย์การจัดการ SharePoint สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการไซต์ในศูนย์การจัดการ SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>เคล็ด

- คุณ **ไม่สามารถ** สร้างไซต์ด้วย URL เดียวกันของไซต์ที่มีอยู่ ถ้าคุณลบไซต์และต้องการใช้ URL ใหม่อาจเป็นไปได้ว่าไซต์ที่ถูกลบจะยังคงอยู่ภายใต้[ไซต์ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) ไซต์จะต้องถูกลบอย่างถาวรเพื่อใช้ URL ใหม่ เมื่อต้องการเอาไซต์ออกด้วย Powershell ให้ดูที่ตัวอย่างของ cmdlet [SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้ [ดูจัดการการสร้างไซต์ใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)
- เป็นไปได้ว่าไซต์จะปรากฏอยู่ที่การ **สร้าง** นานกว่าที่คาดไว้ ถ้าคุณได้รับการส่งผ่านมากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว โปรดแจ้งให้เราทราบอย่างน้อย24ชั่วโมงเพื่อให้โซลูชันเสร็จสมบูรณ์
