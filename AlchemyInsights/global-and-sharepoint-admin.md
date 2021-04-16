---
title: ผู้ดูแลระบบส่วนกลางและ SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: 91abc97be5d616392f8d04b3641af3c9dd8bfd74
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811907"
---
# <a name="global-and-sharepoint-admin"></a>ผู้ดูแลระบบส่วนกลางและ SharePoint

ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint ต้องได้รับการมอบหมายสิทธิ์การใช้งาน SharePoint บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว

ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบส่วนกลางหรือ SharePoint มีสิทธิ์เข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") ระบุผู้ดูแลระบบไซต์ จัดการการตั้งค่าการแชร์ และอื่นๆ พวกเขาไม่มีการเข้าถึงโดยอัตโนมัติไปยังไซต์ทั้งหมดและ OneDrive ของผู้ใช้แต่ละคน แต่พวกเขาสามารถให้ตนเองเข้าถึงไซต์หรือ OneDrive ได้ พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)
มีหลายสาเหตุที่ Microsoft SharePoint หรือ Microsoft OneDrive อาจไม่สามารถเข้าถึงได้ ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คู่มือต่อไปนี้เพื่อแก้ไขปัญหานี้

- [ไม่สามารถเข้าถึง SharePoint Online ได้](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [การเข้าถึงถูกปฏิเสธบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)