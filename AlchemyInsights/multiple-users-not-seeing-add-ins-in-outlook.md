---
title: ผู้ใช้หลายคนไม่เห็น add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729890"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>ผู้ใช้หลายคนไม่เห็น add-in ใน Outlook

ถ้าคุณทดสอบ add-in ของ Outlook และไม่มีการแสดงเป็นขั้นตอนการแก้ไขปัญหาแรกให้ใช้ cmdlet PowerShell**ชื่อ get-organizationconfig**เพื่อสอบถามพารามิเตอร์_AppsForOfficeEnabled_ ถ้าคิวรีส่งกลับค่า **False**ให้ตั้งค่าพารามิเตอร์นี้เป็น **True** โดยใช้ Cmdlet การ **ตั้งค่าชื่อ get-organizationconfig** ดังนั้น add-in จะปรากฏขึ้นตามที่คาดไว้

เราไม่แนะนำให้พารามิเตอร์_AppsForOfficeEnabled_ถูกตั้งค่าเป็น**False** ค่าของ **False** จะแทนที่การตั้งค่าบทบาทของผู้ดูแลระบบและผู้ใช้ทั้งหมดและป้องกันไม่ให้แอปใหม่ถูกเปิดใช้งานโดยผู้ใช้ใดๆในองค์กร

สำหรับข้อมูลเพิ่มเติมให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)ได้