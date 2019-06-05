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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716910"
---
# <a name="sharepoint-designer-connection-issues"></a>ปัญหาการเชื่อมต่อของ SharePoint Designer 

<p>ถ้า SharePoint Designer ประสบปัญหาการเชื่อมต่อไปยังไซต์ SharePoint กรุณาลองแก้ไขปัญหาทั่วไปต่อไปนี้</p> <p><strong>ขั้นตอนที่ 1:</strong> <strong>ตรวจสอบ SharePoint Designer มีการอัพเด&nbsp;</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer การ Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">โปรแกรมปรับปรุงสำหรับโปรแกรมออกแบบ SharePoint 2013 (KB3114721)</a></li> </ul> <p><strong>ขั้นตอนที่ 2:</strong> <strong>ล้างข้อมูลแฟ้มแคชภายในเครื่อง</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">ปิด SharePoint Designer 2013&nbsp;</li> <li style="font-weight: 400;">บนเครื่องคอมพิวเตอร์ เรียกดูไปยังโฟลเดอร์ต่อไปนี้เพื่อลบแฟ้มแคช&nbsp;</li> <li style="font-weight: 400;">คลิ<strong>เริ่มต้น -&gt;รัน</strong>และลบแฟ้มทั้งหมดที่พบภายใต้แต่ละอยู่ด้านล่างตำแหน่งที่ตั้ง&nbsp;<br /><br />Extensions\Cache เซิร์ฟเวอร์ %APPDATA%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูถ้าทำงาน</li> </ol> <p><strong>ขั้นตอนที่ 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide">การ<strong>เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office 2013 บนอุปกรณ์ Windows</strong></a>&nbsp;</p> <p><strong>ขั้นตอนที่ 4:</strong> <strong>ผู้ดูแลจะต้องใช้การอนุญาตให้ใช้สคริปต์แบบกำหนดเองเพื่ออนุญาตการเชื่อมต่อของ SharePoint Designer</strong></p> <p>สำหรับขั้นตอนโดยละเอียด ตัวอย่าง และข้อควรพิจารณาดู<a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง</a>&nbsp;</p>


