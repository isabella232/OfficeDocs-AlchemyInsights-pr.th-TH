---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700474"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จำกัดการเข้าถึงใน SharePoint หรือ OneDrive

มีหลายวิธีในการจำกัดการเข้าถึงบริการ SharePoint Online/OneDrive วิธีการจำกัดการเข้าถึงต่างๆเหล่านี้จะมีการระบุไว้ด้านล่าง 

**ข้อจำกัดสิทธิ์**

ใน SharePoint Online และ OneDrive for Business เราจะจำกัดการเข้าถึงรายการเช่นไซต์ไฟล์และโฟลเดอร์โดยการอนุญาตให้เข้าถึงกลุ่มเหล่านั้น/บุคคลที่ควรมีสิทธิ์เข้าถึงเท่านั้น

- [กำหนดสิทธิ์สำหรับรายการหรือไลบรารี SharePoint เอง](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [กำหนดสิทธิ์ของไซต์ SharePoint เอง](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [การเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [การควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลางคุณสามารถบล็อกหรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ไม่มีการเข้าร่วมโฆษณาแบบไฮบริดหรือเข้ากันได้ใน Intune)

**ข้อจำกัดของตำแหน่งบนเครือข่าย**

ในฐานะผู้ดูแลระบบ IT คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่ายที่กำหนดไว้ที่คุณเชื่อถือได้ ซึ่งเรียกว่านโยบายที่ยึดตามตำแหน่งที่ตั้ง สำหรับข้อมูลเพิ่มเติมโปรดดู [ที่การควบคุมการเข้าถึงข้อมูล SharePoint Online และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**ข้อจำกัดของการล็อกไซต์** 

ภายใน SharePoint Online คุณจะสามารถล็อกไซต์คอลเลกชันได้ดังนั้นจึงไม่มีสิทธิ์ในการเข้าถึง การตั้งค่านี้จะถูกตั้งค่าผ่านทาง PowerShell และการ [จัดการ SharePoint Online Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) โดยใช้คุณสมบัติ [get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState

**จำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**

ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลางคุณสามารถทำให้ผู้ใช้ของคุณสามารถสร้างและจัดการไซต์ SharePoint ของตนเองได้ซึ่งจะกำหนดชนิดของไซต์ที่พวกเขาสามารถสร้างและระบุตำแหน่งที่ตั้งของไซต์ได้ สำหรับข้อมูลเพิ่มเติมโปรดดู [ที่จัดการการสร้างไซต์ใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

