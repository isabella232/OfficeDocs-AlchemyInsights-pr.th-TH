---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707973"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>แก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธในศูนย์การจัดการ Sharepoint/OneDrive

ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้กําหนด [สิทธิ์การใช้งานให้กับ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ผู้ใช้ ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าพวกเขาได้รับมอบหมาย [บทบาทผู้ดูแลระบบ](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ที่สามารถเข้าถึงศูนย์การจัดการ

ปัญหานี้ยังสามารถเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างใหม่ด้วยชื่อหลักของผู้ใช้ (UPN) เดียวกัน บัญชีใหม่จะถูกสร้างขึ้นโดยใช้รหัส PUID (รหัสพาสปอร์ตไม่ซ้ากัน) ค่าอื่น เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีด้วย Active Directory ขององค์กร (OU) ถ้าผู้ใช้ลงชื่อเข้าใช้ SharePoint แล้วและถูกย้ายไปยัง OU อื่นและซิงค์กับ SharePoint อีกครั้ง ผู้ใช้อาจพบปัญหานี้

เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ คืนค่า[ผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานกับผู้ใช้หลายรายที่เคยมีสิทธิ์เข้าถึง อาจมีปัญหาด้านบริการชั่วคราว  [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)


