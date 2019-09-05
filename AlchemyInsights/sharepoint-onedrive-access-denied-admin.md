---
title: การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751295"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive

ถ้าคุณได้รับข้อความที่ถูกปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไปยังศูนย์ดูแล Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ผู้ดูแลระบบ ถ้าผู้ใช้มีใบอนุญาตคุณควรตรวจสอบให้แน่ใจว่ามี[การกำหนดบทบาทผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์ดูแล

ปัญหานี้อาจเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลักเดียวกัน (UPN) บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสเฉพาะที่ไม่ซ้ำกัน) เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ไม่ถูกต้อง สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กรไดเรกทอรีที่ใช้งานอยู่ (OU) ถ้าผู้ใช้มีการลงชื่อเข้าสู่ SharePoint แล้วและถูกย้ายไปยัง OU ที่แตกต่างกันและทำซ้ำกับ SharePoint พวกเขาอาจพบปัญหานี้

เพื่อแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Office ๓๖๕](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)

หมายเหตุ: ถ้าการ OneDrive หรือศูนย์กลางการดูแล SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร  [ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)


