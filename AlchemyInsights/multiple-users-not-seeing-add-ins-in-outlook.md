---
title: ผู้ใช้หลายคนไม่เห็น Add-in ในOutlook
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
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011823"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>ผู้ใช้หลายคนไม่เห็น Add-in ในOutlook

ถ้าคุณทดสอบOutlook Add-in และไม่มี Add-in แสดงขึ้นในขั้นตอนการแก้ไขปัญหาแรก ให้ใช้ cmdlet **Get-OrganizationConfig** PowerShell เพื่อคิวรี _พารามิเตอร์ AppsForOfficeEnabled_ ถ้าคิวรีส่งกลับค่าเป็น **False** ให้ตั้งค่าพารามิเตอร์นี้เป็น **True** โดยใช้ cmdlet **Set-OrganizationConfig** ดังนั้น Add-in จะปรากฏขึ้นตามที่คาดไว้

เราไม่แนะให้ _ตั้งค่าพารามิเตอร์ AppsForOfficeEnabled_ **เป็น** False ค่าของ False **จะ** แทนที่การตั้งค่าบทบาทของผู้ใช้และการดูแลระบบข้างต้นทั้งหมด และป้องกันแอปใหม่จากการเปิดใช้งานโดยผู้ใช้ในองค์กร

For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).