---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511563"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของ SharePoint Designer 

ถ้า SharePoint Designer กําลังประสบปัญหาการเชื่อมต่อกับไซต์ SharePoint โปรดลองวิธีแก้ไขปัญหาทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer 2013 ถูกปรับปรุง ด้วย[SharePoint ออกแบบ Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และ[2 สิงหาคม 2016 ปรับปรุงสําหรับ SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



ขั้นตอนที่ 2: ล้างแฟ้มแคชภายในเครื่อง:

1. ปิด 2013 ตัวออกแบบของ SharePoint

2. บนคอมพิวเตอร์เฉพาะที่ เอาแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้

    - ส่วนขยายของเว็บเซิร์ฟเวอร์\แคช
    - ตัวออกแบบของโปรแกรมประยุกต์%\Microsoft\SharePoint\พร็อกซีแอสเซมบลี
    - %โปรไฟล์ผู้ใช้%\โปรแกรมประยุกต์ข้อมูล\ภายในเครื่อง\Microsoft\เว็บไซต์การแคช

3. เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูว่าใช้งานได้หรือไม่

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง**อนุญาตสคริปต์แบบกําหนดเอง**ในการตั้งค่าศูนย์การจัดการ SharePoint เพื่ออนุญาตให้มีการเชื่อมต่อ SharePoint Designer ดู[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สําหรับข้อมูลเพิ่มเติม


