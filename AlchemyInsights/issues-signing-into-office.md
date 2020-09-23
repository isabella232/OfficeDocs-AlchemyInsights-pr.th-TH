---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236144"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕

เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้ด้วยแอป Microsoft ๓๖๕ให้ลองใช้ตัวเลือกต่อไปนี้บนเครื่องจักรที่ได้รับผลกระทบ:  

- สำหรับ Windows ให้ดู [คำแนะนำเกี่ยวกับการแก้ไขปัญหาทั่วไปในการลงชื่อเข้าใช้](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- สำหรับ Mac ให้ดูที่  [ไม่สามารถลงชื่อเข้าใช้แอป Office ๒๐๑๖ For Mac ได้](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปได้โดยอัตโนมัติสำหรับคุณ ดาวน์โหลดและเรียกใช้ตัว  **[ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา

**หมายเหตุ:** การปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่ (ADAL) หรือการจัดการบัญชีผู้ใช้เว็บ (WAM) สำหรับการแก้ไขปัญหาการลงชื่อเข้าใช้หรือการเปิดใช้งานไม่**แนะนำ** ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Microsoft ๓๖๕โดยใช้ Office ๒๐๑๓ให้ตรวจสอบให้แน่ใจว่าคุณได้ [เปิดใช้งานการรับรองความถูกต้องที่ทันสมัย](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  สำหรับไคลเอ็นต์ Office

สำหรับการดำเนินการแก้ไขปัญหาที่เฉพาะเจาะจงให้ดูที่:

[ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office ๒๐๑๖รุ่น16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[คุณไม่สามารถลงชื่อเข้าใช้บัญชีผู้ใช้ขององค์กรของคุณเช่น Office ๓๖๕, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Office ๓๖๕, Azure หรือ Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[ได้รับพร้อมท์ซ้ำๆสำหรับข้อมูลประจำตัวใน Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)