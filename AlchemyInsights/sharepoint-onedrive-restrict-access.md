---
title: จํากัดการเข้าถึงในSharePointหรือOneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093907"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จํากัดการเข้าถึงในSharePointหรือOneDrive

มีหลายวิธีในการจํากัดการเข้าถึงบริการSharePoint Online/OneDrive วิธีการจํากัดการเข้าถึงต่างๆ เหล่านี้มีระบุไว้ด้านล่าง 

**ข้อจํากัดสิทธิ์**

ใน SharePoint Online และ OneDrive for Business เราจะจํากัดการเข้าถึงรายการต่างๆ เช่น ไซต์ ไฟล์ และโฟลเดอร์ โดยให้สิทธิ์การเข้าถึงไปยังกลุ่ม/บุคคลที่ควรมีสิทธิ์เข้าถึงเท่านั้น

- [การปรับแต่งสิทธิ์SharePointรายการหรือไลบรารี](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [การSharePointสิทธิ์ของไซต์เอง](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [เปลี่ยนสิทธิ์ในโฟลเดอร์ย่อย](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [ควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

ในฐานะผู้ดูแลระบบ SharePointหรือผู้ดูแลระบบส่วนกลาง คุณสามารถบล็อกหรือจํากัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ที่ไม่ได้เข้าร่วมหรือปฏิบัติตามข้อบังคับ AD แบบไฮบริดใน Intuned) ได้

**การจํากัดสถานที่ตั้งเครือข่าย**

ในฐานะผู้ดูแลระบบ IT คุณสามารถควบคุมการเข้าถึงแหล่งข้อมูลSharePoint OneDriveแหล่งข้อมูลที่กําหนดโดยยึดตามสถานที่ตั้งเครือข่ายที่คุณเชื่อถือ หรือเรียกอีกอย่างว่านโยบายตามสถานที่ For more information, please see [Control access to SharePoint online and OneDrive based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**ข้อจํากัดการล็อกไซต์** 

Within SharePoint Online you have theability to lock down a site collection, so no one has access. ซึ่งถูกตั้งค่าผ่าน PowerShell และ SharePoint [Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้คุณสมบัติ[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockStatt

**จํากัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**

ในฐานะSharePointผู้ดูแลระบบหรือผู้ดูแลระบบส่วนกลาง คุณสามารถให้ผู้ใช้ของคุณสร้างและดูแลไซต์ SharePoint ของตนเองได้ ระบุชนิดของไซต์ที่พวกเขาสามารถสร้าง และระบุที่ตั้งของไซต์ได้ For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

