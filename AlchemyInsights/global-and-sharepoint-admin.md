---
title: ส่วนกลางและผู้ดูแลระบบ SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: 231f302bd3f3655b1fe72518d71b14d464914ce0
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716438"
---
# <a name="global-and-sharepoint-admin"></a>ส่วนกลางและผู้ดูแลระบบ SharePoint

ผู้ดูแลระบบส่วนกลางและ SharePoint ต้องได้รับมอบหมายสิทธิ์การใช้งาน SharePoint บัญชีที่สร้างขึ้นใหม่เพิ่งได้รับมอบหมายด้วยบทบาทสิทธิ์การใช้งาน SharePoint หรือผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้อย่างน้อย 24 ชั่วโมงสําหรับการซิงค์เพื่อให้เสร็จสมบูรณ์ในระบบของเรา เราเข้าใจว่า 24 ชั่วโมงอาจดูเหมือนเป็นเวลานาน ในหลายกรณีเรากําลังทํางานอยู่แล้วในการแก้ปัญหา

ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบ Global หรือ SharePoint สามารถเข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") พวกเขาไม่มีการเข้าถึงโดยอัตโนมัติไปยังไซต์ทั้งหมดและ OneDrive ของผู้ใช้แต่ละราย แต่พวกเขาสามารถให้ตัวเองเข้าถึงเว็บไซต์หรือ OneDrive นอกจากนี้ พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูที่[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)
มีหลายสาเหตุที่ทําให้ Microsoft SharePoint หรือ Microsoft OneDrive ไม่สามารถเข้าถึงได้ ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คําแนะนําต่อไปนี้เพื่อแก้ไขปัญหานี้

- [ไม่สามารถเข้าถึง SharePoint แบบออนไลน์ได้](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [การเข้าถึงถูกปฏิเสธสําหรับบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)