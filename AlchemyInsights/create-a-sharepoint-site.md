---
title: สร้างไซต์ SharePoint
ms.author: pebaum
author: todmccoy
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
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770874"
---
# <a name="create-a-sharepoint-site"></a>สร้างไซต์ SharePoint

สร้างหรือจัดการไซต์จาก[ไซต์ที่ใช้งานอยู่](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)ในศูนย์ดูแล SharePoint สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การจัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>เคล็ด ลับ:

- คุณ**ไม่สามารถ**สร้างไซต์ที่มี URL เดียวกันของไซต์ที่มีอยู่ ถ้าคุณลบไซต์และต้องการใช้ URL อีกครั้งอาจเป็นไปได้ว่าไซต์ที่ถูกลบนั้นยังคงอยู่ภายใต้[ไซต์ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) ไซต์จะต้องถูกลบออกอย่างถาวรเพื่อใช้ URL อีกครั้ง เมื่อต้องการเอาไซต์ออกด้วย Powershell ให้ดูที่ตัวอย่างของ cmdlet [SPSite เอาออก](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้ [ดูจัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)
- มันเป็นไปได้ว่าเว็บไซต์ปรากฏติดอยู่ที่การ**สร้าง**นานกว่าที่คาดไว้ ถ้ามากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน ในหลายกรณีเรากำลังหาทางแก้ไขปัญหาอยู่ กรุณาให้เราอย่างน้อย24ชั่วโมงเพื่อให้การแก้ไขปัญหา
