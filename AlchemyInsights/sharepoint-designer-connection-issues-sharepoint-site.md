---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840570"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของ SharePoint Designer 

ถ้า SharePoint Designer ประสบปัญหาการเชื่อมต่อไปยังไซต์ SharePoint กรุณาลองแก้ไขปัญหาทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบว่า มีการปรับปรุง SharePoint Designer 2013 มีค่า[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 สิงหาคม 2016 ปรับปรุง SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



ขั้นตอนที่ 2: ลบแฟ้มแคชภายในเครื่อง:

1. ปิด SharePoint Designer 2013

2. บนเครื่องคอมพิวเตอร์ ลบแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้

    - Extensions\Cache เซิร์ฟเวอร์ %APPDATA%\Microsoft\Web
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูถ้าทำงาน

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

ขั้นตอนที่ 4: ผู้ดูแลจะต้อง**อนุญาตให้สคริปต์แบบกำหนดเอง**ในการตั้งค่าศูนย์กลางการดูแล SharePoint เพื่ออนุญาตการเชื่อมต่อของ SharePoint Designer ดู[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สำหรับข้อมูลเพิ่มเติม


