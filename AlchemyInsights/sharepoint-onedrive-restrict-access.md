---
title: จํากัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692784"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จํากัดการเข้าถึงใน SharePoint หรือ OneDrive

มีหลายวิธีในการจํากัดการเข้าถึงบริการแบบออนไลน์/OneDrive ของ SharePoint วิธีการจํากัดการเข้าถึงต่างๆ เหล่านี้มีรายละเอียดด้านล่าง 

**ข้อจํากัดสิทธิ์**

ใน SharePoint Online และ OneDrive สําหรับธุรกิจ เราจํากัดการเข้าถึงรายการต่างๆ เช่น ไซต์ ไฟล์ และโฟลเดอร์โดยการอนุญาตให้เข้าถึงกลุ่ม/บุคคลที่ควรมีสิทธิ์เข้าถึงเท่านั้น

- [กําหนดสิทธิ์สําหรับไลบรารีหรือรายการ SharePoint เอง](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [การกําหนดสิทธิ์สําหรับไซต์ SharePoint เอง](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [เปลี่ยนสิทธิ์บนโฟลเดอร์ย่อย](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [ควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

ในฐานะ SharePoint หรือผู้ดูแลระบบส่วนกลาง คุณสามารถบล็อกหรือจํากัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ผู้ที่ไม่ไฮบริดโฆษณาเข้าร่วมหรือเข้ากันได้ใน Intune)

**การจํากัดตําแหน่งบนเครือข่าย**

ในฐานะผู้ดูแลระบบ IT คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive ตามตําแหน่งที่ตั้งเครือข่ายที่กําหนดที่คุณเชื่อถือ ซึ่งเรียกว่านโยบายตามตําแหน่งที่ตั้ง สําหรับข้อมูลเพิ่มเติม โปรดดู[ควบคุมการเข้าถึงแบบออนไลน์ของ SharePoint และ OneDrive ข้อมูลตามตําแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**ข้อจํากัดการล็อกไซต์** 

ภายใน SharePoint Online คุณสามารถล็อกไซต์คอลเลกชันได้ ตั้งค่านี้ผ่านทาง PowerShell และ[เชลล์จัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้การตั้งค่า[SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState คุณสมบัติ

**จํากัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**

ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลาง สําหรับข้อมูลเพิ่มเติม โปรดดู[การจัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)

