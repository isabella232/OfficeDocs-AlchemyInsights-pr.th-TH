---
title: การแก้ไขปัญหาการเข้าถึงข้อความถูกปฏิเสธ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085247"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงข้อความถูกปฏิเสธในศูนย์การจัดการ sharepoint/OneDrive

ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้กําหนดสิทธิ์การใช้งาน[ให้กับ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ผู้ใช้ ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าพวกเขาได้รับมอบหมาย [บทบาทผู้ดูแลระบบ](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ที่สามารถเข้าถึงศูนย์การจัดการได้

ปัญหานี้ยังอาจเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างใหม่ด้วยชื่อหลักของผู้ใช้ (UPN) เดียวกัน บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสพาสปอร์ตเฉพาะ) ค่าอื่น เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือOneDriveของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีด้วยหน่วยขององค์กร Active Directory (OU) ถ้าผู้ใช้ลงชื่อเข้าใช้ใน SharePoint แล้วถูกย้ายไปยัง OU อื่นและซิงค์กับ SharePoint อีกครั้ง ผู้ใช้อาจประสบปัญหานี้

เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ คืนค่า[ผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)ใน Microsoft 365

หมายเหตุ: ถ้าOneDriveหรือSharePointผู้ดูแลระบบของคุณไม่พร้อมให้ใช้งานกับผู้ใช้หลายคนที่เคยเข้าถึง อาจมีปัญหาด้านบริการชั่วคราว  [ตรวจสอบแดชบอร์ดสถานภาพ](https://portal.office.com/adminportal/home#/servicehealth)บริการ


