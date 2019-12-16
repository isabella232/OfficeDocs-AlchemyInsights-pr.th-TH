---
title: ปัญหาการเชื่อมต่อของตัวออกแบบ SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051732"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของตัวออกแบบ SharePoint 

ถ้า SharePoint Designer กำลังประสบกับปัญหาการเชื่อมต่อไปยังไซต์ SharePoint โปรดลองใช้โซลูชันทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer ๒๐๑๓ถูกปรับปรุงด้วยตัว[ออกแบบ Sharepoint Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และ[2 สิงหาคม๒๐๑๖การปรับปรุงสำหรับ SharePoint Designer ๒๐๑๓](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



ขั้นตอนที่ 2: ล้างไฟล์แคชภายในเครื่อง:

1. ปิดตัวออกแบบ SharePoint ๒๐๑๓

2. บนคอมพิวเตอร์เฉพาะที่ให้เอาแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้ออก

    - \ การขยายการเว็บเซิร์ฟเวอร์ \
    - \ '% \Nat\ \ ' \
    - \Napa\nater\ \

3. เปิด SharePoint Designer ๒๐๑๓และป้อนบัญชีอีกครั้งเพื่อดูว่าการทำงานหรือไม่

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง**อนุญาตให้สคริปต์ที่กำหนดเอง**ในการตั้งค่าศูนย์ดูแล sharepoint เพื่ออนุญาตให้มีการเชื่อมต่อ SharePoint Designer โปรดดูที่[อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สำหรับข้อมูลเพิ่มเติม


