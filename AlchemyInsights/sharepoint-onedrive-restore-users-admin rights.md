---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยังไซต์ OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670635"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยังไซต์ OneDrive for Business

ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน บัญชีผู้ใช้ใหม่ถูกสร้างโดยใช้ค่า PUID (ID ที่ไม่ซ้ำกันของ Passport) ที่แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองจะเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีกับหน่วยองค์กร Active Directory (OU) ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint เรียบร้อยแล้วและจะถูกย้ายไปยัง OU และ resynced ที่แตกต่างกันกับ SharePoint พวกเขาอาจประสบปัญหานี้

1. เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN ต้นฉบับที่มีขั้นตอนในบทความให้[คืนค่าผู้ใช้ใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมที่คุณควรเอาผู้ใช้เก่าออกจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้ให้[เอาผู้ใช้ออกจากรายการข้อมูลผู้ใช้]() 
3. หลังจากเสร็จเรียบร้อยแล้วคุณสามารถตรวจสอบว่าผู้ใช้มีสิทธิ์ผู้ดูแลระบบไปยังไซต์ OneDrive โดยทำตามขั้นตอนในการ [เพิ่มผู้ดูแลระบบสำหรับ onedrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ให้ดูบทความการ[ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
