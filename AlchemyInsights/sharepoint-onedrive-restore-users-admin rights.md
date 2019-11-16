---
title: การแก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธไปยัง OneDrive สำหรับไซต์ธุรกิจ
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766730"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธไปยัง OneDrive สำหรับไซต์ธุรกิจ

ปัญหานี้มักเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสเฉพาะที่ไม่ซ้ำกัน) เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ไม่ถูกต้อง สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กรไดเรกทอรีที่ใช้งานอยู่ (OU) ถ้าผู้ใช้มีการลงชื่อเข้าสู่ SharePoint แล้วและถูกย้ายไปยัง OU ที่แตกต่างกันและทำซ้ำกับ SharePoint พวกเขาอาจพบปัญหานี้

1. เพื่อแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Office ๓๖๕](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมคุณควรเอาผู้ใช้เก่าจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้[เอาผู้ใช้ออกจากรายการข้อมูลผู้ใช้]() 
3. หลังจากนี้เสร็จสิ้นคุณสามารถตรวจสอบผู้ใช้มีสิทธิ์ของผู้ดูแลระบบไปยังไซต์ OneDrive ได้โดยทำตามขั้นตอนเพื่อ[เพิ่มผู้ดูแลสำหรับ OneDrive ของ](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)คุณ

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ให้ดูบทความให้[เข้าใจระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
