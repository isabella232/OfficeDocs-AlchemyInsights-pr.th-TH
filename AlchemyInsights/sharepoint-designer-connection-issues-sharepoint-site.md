---
title: ระดับสิทธิ์ SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760711"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของ SharePoint Designer 

ถ้า SharePoint Designer ประสบปัญหาการเชื่อมต่อไปยังไซต์ SharePoint กรุณาลองแก้ไขปัญหาทั่วไปต่อไปนี้

ขั้นตอนที่ 1: ตรวจสอบ SharePoint Designer ถูกปรับปรุง

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer การ Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [โปรแกรมปรับปรุงสำหรับโปรแกรมออกแบบ SharePoint 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

ขั้นตอนที่ 2: ลบแฟ้มแคชภายในเครื่อง

- ปิด SharePoint Designer 2013

- บนเครื่องคอมพิวเตอร์ เรียกดูไปยังโฟลเดอร์ต่อไปนี้เพื่อลบแฟ้มแคช

- คลิกเริ่มต้น การเรียกใช้และลบแฟ้มทั้งหมดที่พบภายใต้แต่ละอยู่ด้านล่างตำแหน่งที่ตั้ง

เซิร์ฟเวอร์ %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูถ้าทำงาน

ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

ขั้นตอนที่ 4: ผู้ดูแลจะต้องใช้เมื่อต้องการอนุญาตให้ใช้สคริปต์แบบกำหนดเองเพื่ออนุญาตการเชื่อมต่อของ SharePoint Designer

สำหรับขั้นตอนโดยละเอียด ตัวอย่าง และข้อควรพิจารณาดู[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


