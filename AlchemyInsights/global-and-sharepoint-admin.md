---
title: ผู้ดูแลระบบส่วนกลางSharePointผู้ดูแลระบบ
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
ms.openlocfilehash: 03a76d22f1370234442afe455b4b898a37dd796b7d795c7ab1190ddd3102ae11
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056437"
---
# <a name="global-and-sharepoint-admin"></a>ผู้ดูแลระบบส่วนกลางSharePointผู้ดูแลระบบ

ผู้ดูแลระบบส่วนกลางSharePointและผู้ดูแลระบบต้องได้รับการSharePointสิทธิ์การใช้งานของคุณ บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePointหรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึงSharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว

ผู้ใช้ที่ได้รับการมอบหมายบทบาทผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint มีสิทธิ์เข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") มอบหมายผู้ดูแลไซต์ จัดการการตั้งค่าการแชร์ และอื่นๆ พวกเขาไม่มีการเข้าถึงโดยอัตโนมัติไปยังไซต์ทั้งหมดและไซต์ของผู้ใช้แต่ละคน OneDrive แต่พวกเขาสามารถให้ตนเองสามารถเข้าถึงไซต์หรือOneDriveได้ นอกจากนี้ พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อSharePointและOneDriveได้

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[เกี่ยวกับSharePointผู้ดูแลระบบใน Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)
มีหลายสาเหตุที่ Microsoft SharePointหรือMicrosoft OneDriveอาจไม่สามารถเข้าถึงได้ ถ้าคุณไม่สามารถเข้าถึงแอป SharePoint Online ให้ใช้คู่มือต่อไปนี้เพื่อแก้ไขปัญหานี้

- [ไม่สามารถเข้าถึงบัญชีSharePointออนไลน์](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [การเข้าถึงถูกปฏิเสธบัญชีผู้ใช้ที่มีการจัดการ PIM ในSharePointหรือOneDriveการจัดการ](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)