---
title: ผู้ใช้หลายคนไม่เห็น Add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198244"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>ผู้ใช้หลายคนไม่เห็น Add-in ใน Outlook

ถ้าคุณทดสอบโปรแกรม Outlook add-in และ none ปรากฏขึ้น เป็นขั้นตอนการแก้ไขปัญหาแรก ใช้ cmdlet รับ**OrganizationConfig** PowerShell การสอบถามพารามิเตอร์_AppsForOfficeEnabled_ ถ้าแบบสอบถามส่งกลับค่า**ของเท็จ**ตั้งค่าพารามิเตอร์นี้เป็น**Truy**โดยใช้ cmdlet **Set-OrganizationConfig**ดังนั้น add-ins ปรากฏตามที่คาดไว้

เราไม่แนะนําให้พารามิเตอร์_AppsForOfficeEnabled_ถูกตั้งค่าเป็น**เท็จ** ค่าของ**False**จะแทนที่การตั้งค่าบทบาทผู้ดูแลระบบและผู้ใช้ข้างต้นทั้งหมด และป้องกันไม่ให้ผู้ใช้ใด ๆ ในองค์กรเปิดใช้งานแอปใหม่

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ Add-in สําหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)