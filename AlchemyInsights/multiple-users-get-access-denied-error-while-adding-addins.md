---
title: ผู้ใช้หลายคนได้รับข้อผิดพลาดในการปฏิเสธการเข้าถึงในขณะที่เพิ่ม add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724382"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>ผู้ใช้หลายคนได้รับข้อผิดพลาดในการปฏิเสธการเข้าถึงในขณะที่เพิ่ม add-in ใน Outlook

คุณสามารถระบุว่าผู้ดูแลระบบใดในองค์กรของคุณมีสิทธิ์ในการติดตั้งและจัดการ add-in สำหรับ Outlook นอกจากนี้คุณยังสามารถระบุผู้ใช้ที่อยู่ในองค์กรของคุณได้รับสิทธิ์ในการติดตั้งและจัดการ add-in สำหรับการใช้งานของตนเอง

สำหรับรายละเอียดให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)ได้

เมื่อต้องการตรวจสอบว่าคุณได้กำหนดสิทธิ์สำหรับผู้ใช้ให้แทนที่ <Role Name> ด้วยชื่อของบทบาทเพื่อตรวจสอบและเรียกใช้คำสั่งต่อไปนี้ใน Exchange Online PowerShell:

รับ-ManagementRoleAssignment-บทบาท " <Role Name> "-GetEffectiveUsers

ตัวอย่างนี้จะแสดงให้คุณเห็นวิธีการตรวจสอบว่าคุณได้กำหนดสิทธิ์ในการติดตั้ง add-in จาก Office Store สำหรับองค์กรหรือไม่

PowerShell

-บทบาท "แอป Org Marketplace"-GetEffectiveUsers

ในผลลัพธ์ที่ได้รับ ManagementRoleAssignment ให้ตรวจทานรายการในคอลัมน์ผู้ใช้ที่มีประสิทธิภาพ

สำหรับรายละเอียดเกี่ยวกับไวยากรณ์และพารามิเตอร์ข้อมูลให้ดูที่[รับ ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)
 