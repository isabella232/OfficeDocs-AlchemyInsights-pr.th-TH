---
title: ลบไซต์ใน SharePoint อย่างถาวร
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
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771740"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>ลบไซต์ใน SharePoint อย่างถาวร

เมื่อต้องการนำ URL มาใช้ใหม่จากไซต์ที่ถูกลบ (เมื่อต้องการสร้างไซต์ใหม่) หรือเมื่อต้องการลบไซต์อย่างถาวรเนื่องจากไม่มีการใช้งานอีกต่อไปคุณสามารถใช้การ **ลบอย่างถาวร** จากศูนย์การจัดการ SharePoint ใหม่ได้ 

1. ไปที่ [หน้าไซต์ที่ถูกลบของศูนย์การจัดการ SharePoint ใหม่](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) แล้วลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีสิทธิ์ผู้ดูแลระบบสำหรับองค์กรของคุณ 

2. ในคอลัมน์ด้านซ้ายให้เลือกไซต์ 

3. คลิก**ลบอย่างถาวร** 

**หมายเหตุ**: ไม่สามารถลบไซต์ที่เชื่อมต่อกับกลุ่มได้อย่างถาวรจากศูนย์การจัดการ SharePoint ใหม่ [เอาออก-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) จะต้องถูกใช้แทน  

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ลบไซต์อย่างถาวร](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) 
