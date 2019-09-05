---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750683"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จำกัดการเข้าถึงใน SharePoint หรือ OneDrive

มีหลายวิธีในการจำกัดการเข้าถึงบริการ SharePoint แบบออนไลน์/OneDrive วิธีการจำกัดการเข้าถึงต่างๆเหล่านี้มีการระบุไว้ด้านล่าง 

**ข้อจำกัดสิทธิ์**

ใน SharePoint แบบออนไลน์และ OneDrive สำหรับธุรกิจเราจำกัดการเข้าถึงรายการต่างๆเช่นไซต์แฟ้มและโฟลเดอร์โดยการให้สิทธิ์เข้าถึงกลุ่มเหล่านั้น/บุคคลที่ควรมีการเข้าถึง

- [กำหนดสิทธิ์สำหรับรายการหรือไลบรารี SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [การกำหนดสิทธิ์ของไซต์ SharePoint เอง](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [การเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [ควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

ในฐานะที่เป็น SharePoint หรือผู้ดูแลส่วนกลางใน Office ๓๖๕คุณสามารถบล็อกหรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ผู้ที่ไม่ได้เป็นสมาชิกไฮบริดสลีเข้าร่วมหรือสอดคล้องกันใน Intune)

**ข้อจำกัดตำแหน่งเครือข่าย**

ในฐานะที่เป็นผู้ดูแลระบบไอทีคุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive ตามตำแหน่งบนเครือข่ายที่กำหนดไว้ที่คุณเชื่อถือได้ ซึ่งเรียกอีกอย่างว่านโยบายตามตำแหน่งที่ตั้ง สำหรับข้อมูลเพิ่มเติมโปรดดู[การควบคุมการเข้าถึงข้อมูล SharePoint แบบออนไลน์และ OneDrive ตามตำแหน่งบนเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**ข้อจำกัดในการล็อกเว็บไซต์** 

ภายใน SharePoint แบบออนไลน์คุณมีความสามารถในการล็อกชุดเก็บรวบรวมไซต์ดังนั้นไม่มีใครมีการเข้าถึง นี้ถูกตั้งค่าผ่านทาง PowerShell และ[เชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้คุณสมบัติการ[ตั้งค่าเว็บไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)-lockstate

**การจำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**

ในฐานะที่เป็นผู้ดูแลระบบ SharePoint หรือ Office ๓๖๕ผู้ดูแลส่วนกลางคุณสามารถให้ผู้ใช้ของคุณสร้างและดูแลไซต์ SharePoint ของตนเองได้กำหนดชนิดของไซต์ที่พวกเขาสามารถสร้างและระบุตำแหน่งที่ตั้งของไซต์ สำหรับข้อมูลเพิ่มเติมโปรดดู[จัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)

