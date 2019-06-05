---
title: ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715230"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN) สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU) ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">คืนค่าผู้ใช้ใน Office 365</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">หลังจากทำเช่นนี้ คุณสามารถตรวจสอบผู้ใช้มีสิทธิ์การดูแลไปยังไซต์ OneDrive โดยทำตามขั้นตอนในการ<a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">เพิ่มของผู้ดูแลระบบสำหรับ OneDrive ของผู้ใช้ได้</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูที่บทความ<a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint</a>&nbsp;</span></p>
