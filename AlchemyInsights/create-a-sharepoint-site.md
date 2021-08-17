---
title: สร้างSharePointไซต์
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080909"
---
# <a name="create-a-sharepoint-site"></a>สร้างSharePointไซต์

สร้างหรือจัดการไซต์[จากไซต์](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)ที่ใช้งานอยู่ในSharePointการจัดการ For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>เคล็ดลับ:

- **คุณไม่สามารถ** สร้างไซต์ที่มี URL เดียวกันของไซต์ที่มีอยู่ได้ ถ้าคุณลบไซต์และต้องการใช้ URL อีกครั้ง อาจเป็นไปได้ว่าไซต์ที่ถูกลบยังคงมีอยู่ภายใต้ ไซต์[ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) ไซต์จะต้องถูกลบอย่างถาวรเพื่อใช้ URL อีกครั้ง เมื่อต้องการเอาไซต์ออกโดยสมบูรณ์ด้วย Powershell ให้ดู[ตัวอย่าง cmdlet Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- ผู้ใช้บางคนอาจไม่สามารถสร้างไซต์ได้ [ดู จัดการการสร้างไซต์ SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)
- อาจเป็นไปได้ว่าไซต์อาจค้างอยู่ที่ **การสร้าง** นานกว่าที่คาดไว้ หากคุณเห็นปัญหานี้เกิน 24 ชั่วโมง โปรดบันทึกตั๋วการสนับสนุน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว โปรดให้เวลาเราอย่างน้อย 24 ชั่วโมงเพื่อแก้ไขปัญหาให้เสร็จสิ้น
