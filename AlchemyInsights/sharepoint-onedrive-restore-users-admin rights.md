---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692820"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ

ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบ และสร้างใหม่ ด้วยชื่อหลัก (UPN) เดียวกัน บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะของ Passport) ที่แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของตนเอง สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับ Active Directory องค์กรหน่วย (OU) ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้

1. เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่างๆ ในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมที่คุณควรเอาผู้ใช้เก่าจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้[Remove a user from the user info list]() 
3. หลังจากเสร็จสิ้นคุณสามารถตรวจสอบว่า ผู้ใช้มีสิทธิ์ของผู้ดูแลระบบไปยังไซต์ OneDrive โดยทําตามขั้นตอนใน[การเพิ่มผู้ดูแลระบบสําหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูที่บทความ การ[ทําความเข้าใจระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
