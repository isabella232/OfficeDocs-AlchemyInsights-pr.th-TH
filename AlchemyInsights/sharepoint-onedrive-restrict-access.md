---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735161"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จำกัดการเข้าถึงใน SharePoint หรือ OneDrive

มีหลายวิธีในการจำกัดการเข้าถึงบริการ ออนไลน์/OneDrive ของ SharePoint วิธีเข้าถึงข้อจำกัดต่าง ๆ จะถูกทำเค้าร่างด้านล่าง 

การจำกัดสิทธิ์

ใน SharePoint แบบออนไลน์และ OneDrive สำหรับธุรกิจ เราจำกัดการเข้าถึงรายการอย่างเช่นไซต์ แฟ้ม และโฟลเดอร์ โดยเฉพาะ สิทธิการเข้าถึงกลุ่ม/ผู้ใช้เหล่านั้นควรมีการเข้าถึง

[กำหนดสิทธิ์สำหรับรายการ SharePoint หรือไลบรารี](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[กำหนดสิทธิ์ของไซต์ SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[เปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[ควบคุมการเข้าถึงจากอุปกรณ์ไม่มีการจัดการ](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

เป็นผู้ดูแลส่วนกลางใน Office 365 หรือ SharePoint คุณสามารถบล็อก หรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ไม่มีการจัดการ (เหล่าไฮบริโฆษณาที่นำมารวมกัน หรือเข้ากันได้ใน Intune) ได้

ข้อจำกัดของตำแหน่งที่ตั้งเครือข่าย

เป็นผู้ดูแลระบบ IT ผิด คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่ายที่กำหนดที่คุณเชื่อถือ นี่คือหรือที่เรียกอีกอย่างหนึ่งว่านโยบายที่อ้างอิงตำแหน่งที่ตั้ง สำหรับข้อมูลเพิ่มเติม โปรดดูที่[ควบคุมการเข้าถึงแบบออนไลน์ของ SharePoint และข้อมูล OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

ข้อจำกัดการล็อกไซต์ 

ภายใน SharePoint แบบออนไลน์ คุณมีความสามารถในการล็อกไซต์คอลเลกชัน เพื่อให้ไม่มีผู้ใดมีสิทธิ์เข้าถึง การกระทำนี้จะตั้งผ่านทาง PowerShell และ[เชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้คุณสมบัติ[ชุด-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState

จำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย

เป็นผู้ดูแลระบบ SharePoint หรือผู้ดูแลส่วนกลางของ Office 365 คุณสามารถให้ผู้ใช้ของคุณสร้าง และการดูแลไซต์ SharePoint ของตนเอง กำหนดชนิดของไซต์ที่พวกเขาสามารถสร้าง และระบุที่ตั้งของไซต์ได้ สำหรับข้อมูลเพิ่มเติม โปรดดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

