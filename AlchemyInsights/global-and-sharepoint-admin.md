---
title: ผู้ดูแลระบบส่วนกลางและ SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: 9d4c5da8b6dc78aa18fd29589495b77b7d835aba
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706394"
---
# <a name="global-and-sharepoint-admin"></a>ผู้ดูแลระบบส่วนกลางและ SharePoint

ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน SharePoint บัญชีผู้ใช้ที่สร้างขึ้นใหม่เพิ่งมอบหมายให้กับสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "access denied" หรือ "ไม่พบผู้ใช้" โปรดให้การซิงค์อย่างน้อย24ชั่วโมงเพื่อให้เสร็จสมบูรณ์ในระบบของเรา เราเข้าใจว่า24ชั่วโมงอาจดูเหมือนเป็นเวลานาน ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว

ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบส่วนกลางหรือ SharePoint จะมีสิทธิ์เข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ได้ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") ที่กำหนดผู้ดูแลไซต์จัดการการตั้งค่าการแชร์และอื่นๆ พวกเขาไม่มีการเข้าถึงไซต์ทั้งหมดโดยอัตโนมัติและ OneDrive ของผู้ใช้แต่ละคนแต่พวกเขาสามารถให้สิทธิ์การเข้าถึงไซต์หรือ OneDrive ของผู้ใช้ได้ นอกจากนี้พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive ได้อีกด้วย

เมื่อต้องการเรียนรู้เพิ่มเติมให้ดู[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft ๓๖๕](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)
มีเหตุผลหลายประการที่ Microsoft SharePoint หรือ Microsoft OneDrive อาจไม่สามารถเข้าถึงได้ ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คำแนะนำต่อไปนี้เพื่อแก้ไขปัญหานี้

- [ไม่สามารถเข้าถึง SharePoint Online ได้](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [การเข้าถึงถูกปฏิเสธสำหรับบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)