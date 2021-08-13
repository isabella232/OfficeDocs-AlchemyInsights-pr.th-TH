---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความOneDrive for Businessไซต์
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957812"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความOneDrive for Businessไซต์

ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบและสร้างใหม่ด้วยชื่อหลักของผู้ใช้เดียวกัน (UPN) บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสพาสปอร์ตเฉพาะ) ค่าอื่น เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือOneDriveของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีด้วยหน่วยขององค์กร Active Directory (OU) ถ้าผู้ใช้ลงชื่อเข้าใช้ใน SharePoint แล้วถูกย้ายไปยัง OU อื่นและซิงค์กับ SharePoint อีกครั้ง ผู้ใช้อาจประสบปัญหานี้

1. เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ คืนค่า[ผู้ใช้ใน](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365
2. ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมได้ คุณควรเอาผู้ใช้เก่าออกจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้ เอา[ผู้ใช้ออกจากรายการ]()ข้อมูลผู้ใช้ 
3. หลังจากเสร็จสิ้นคุณสามารถตรวจสอบว่าผู้ใช้มีสิทธิ์ผู้ดูแลระบบในไซต์ OneDrive โดยปฏิบัติตามขั้นตอนในการ เพิ่ม[ผู้ดูแลระบบ ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)OneDrive

For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
