---
title: SharePoint ปัญหาการเชื่อมต่อตัวออกแบบ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942044"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint ปัญหาการเชื่อมต่อตัวออกแบบ 

ถ้าคุณSharePoint Designer พบปัญหาการเชื่อมต่อไปยังSharePointไซต์ของคุณ โปรดลองใช้วิธีแก้ไขปัญหาทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer 2013 ได้รับการอัปเดตด้วย[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และการอัปเดตวันที่ 2 สิงหาคม[2016 SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



ขั้นตอนที่ 2: ล้างไฟล์แคชภายในเครื่อง:

1. ปิด SharePoint Designer 2013

2. บนคอมพิวเตอร์เฉพาะที่ ให้เอาไฟล์ทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้ออก

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. เปิด SharePoint Designer 2013 แล้วใส่บัญชีอีกครั้งเพื่อดูว่าใช้งานได้หรือไม่

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องOffice 2013 Windowsบนอุปกรณ์](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)ของคุณ

ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง อนุญาต **สคริปต์แบบSharePoint** การตั้งค่าศูนย์การจัดการ SharePoint Designer ดู [อนุญาตหรือป้องกันสคริปต์แบบ](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) ปรับแต่งเอง เพื่อดูข้อมูลเพิ่มเติม


