---
title: การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความ OneDrive สำหรับไซต์ทางธุรกิจ
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507830"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความ OneDrive สำหรับไซต์ทางธุรกิจ

ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN) สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU) ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้

1. เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ[การคืนค่าผู้ใช้ใน Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. ถ้าคุณไม่สามารถคืนค่าที่ผู้ใช้เดิม คุณควรเก่าเอาผู้ใช้ออกจากไซต์ OneDrive โดยใช้ขั้นตอนต่อไป[เอาผู้ใช้จากรายการข้อมูลผู้ใช้]() 
3. หลังจากทำเช่นนี้ คุณสามารถตรวจสอบว่า ผู้ใช้มีสิทธิ์การดูแลไปยังไซต์ OneDrive โดยทำตามขั้นตอนเพื่อ[เพิ่ม admin ของสำหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ดูบทความ[การทำความเข้าใจระดับของสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
