---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727190"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของ SharePoint Designer 

ถ้า SharePoint Designer กำลังประสบปัญหาการเชื่อมต่อกับไซต์ SharePoint โปรดลองใช้วิธีแก้ไขปัญหาทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer ๒๐๑๓ได้รับการอัปเดตด้วย[Sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และการ[อัปเดตประจำเดือนสิงหาคม 2, ๒๐๑๖สำหรับ SharePoint Designer ๒๐๑๓](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



ขั้นตอนที่ 2: ล้างไฟล์แคชภายในเครื่อง:

1. ปิด SharePoint Designer ๒๐๑๓

2. บนคอมพิวเตอร์ที่ใช้อยู่ให้เอาไฟล์ทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้ออก

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. เปิด SharePoint Designer ๒๐๑๓แล้วใส่บัญชีผู้ใช้อีกครั้งเพื่อดูว่าทำงานหรือไม่

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องที่ทันสมัยสำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง **อนุญาตสคริปต์แบบกำหนดเอง** ในการตั้งค่าศูนย์การจัดการ sharepoint เพื่ออนุญาตให้มีการเชื่อมต่อ sharepoint Designer ให้ดูที่ [อนุญาตหรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) สำหรับข้อมูลเพิ่มเติม


