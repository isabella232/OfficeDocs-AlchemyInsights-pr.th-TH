---
title: การสร้างไซต์ SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769610"
---
# <a name="create-a-sharepoint-site"></a>การสร้างไซต์ SharePoint

คุณสามารถดูข้อมูลเกี่ยวกับการสร้างไซต์ SharePoint ต่อไปนี้:
- [จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation): เรียนรู้เกี่ยวกับตัวเลือกการสร้างไซต์รวมถึงวิธีการสร้างไซต์คลาสสิกหรือไซต์ทีมที่ไม่มีกลุ่ม Office ๓๖๕
- [สร้างไซต์ทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): เรียนรู้วิธีการสร้างไซต์ทีม
- [สร้างไซต์การสื่อสารใน SharePoint แบบออนไลน์](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): เรียนรู้วิธีการสร้างไซต์การสื่อสาร
- [จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): เรียนรู้วิธีการสร้างไซต์คลาสสิกหรือไซต์ทีมที่ไม่มีกลุ่ม Office ๓๖๕


  
**เคล็ด ลับ:**
- คุณไม่สามารถสร้างไซต์ที่มี URL เดียวกันของไซต์ที่มีอยู่ได้ หากคุณลบไซต์และต้องการใช้ URL อีกครั้งอาจเป็นไปได้ว่าไซต์ที่ถูกลบยังคงอยู่ภายใต้**ไซต์ที่ถูกลบ** หากต้องการจัดการไซต์ที่ถูกลบให้เห็นให้[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) หากต้องการเอาเว็บไซต์ที่มี Powershell ออกให้ดูตัวอย่างการ[เอาออก spsite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet
- ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้ ดู[จัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)
- เป็นไปได้ที่เว็บไซต์จะปรากฏติดอยู่ที่**การสร้าง**นานกว่าที่คาดไว้ หากมีการผ่านมากกว่า24ชั่วโมงตั้งแต่แรกคุณเห็นปัญหานี้โปรดบันทึกตั๋วสนับสนุน ในหลายกรณีเรากำลังทำงานอยู่แล้วในการแก้ปัญหา กรุณาให้เราอย่างน้อย24ชั่วโมงในการดำเนินการแก้ปัญหา
- ถ้าคุณต้องการสร้างไซต์ทีมใหม่ที่ไม่มีกลุ่ม Office ๓๖๕ 


