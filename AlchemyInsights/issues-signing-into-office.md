---
title: ปัญหาในการลงชื่อเข้าใช้Microsoft 365แอปของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744665"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>ปัญหาในการลงชื่อเข้าใช้Microsoft 365 Apps

หมายเหตุ: ถ้าคุณใช้งาน Windows เวอร์ชันที่เก่ากว่า (เช่น Windows 7 SP1, Windows Server 2008 R2) ให้ใช้การแก้ไขง่ายๆ เพื่อ[](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)เปิดใช้งาน TLS 1.2 เป็นค่าเริ่มต้น For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้Microsoft 365แอปของคุณ ให้ลองตัวเลือกต่อไปนี้บนเครื่องที่ได้รับผลกระทบ:  

- ดูข้อมูลWindowsโปรดดู[รายการแนะนำแก้ไขปัญหาทั่วไปในการลงชื่อเข้าใช้](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- For Mac, [see Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**เคล็ดลับ** บนเครื่องWindows อัตโนมัติ เราสามารถวินิจฉัยและแก้ไขปัญหาการOfficeลงชื่อเข้าใช้ทั่วไปหลายอย่างให้คุณโดยอัตโนมัติ ดาวน์โหลดและเรียกใช้ **[Microsoft ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา

**หมายเหตุ:** ไม่แนะให้ปิดใช้งานการรับรองความถูกต้องสมัยใหม่ (ADAL) หรือการจัดการบัญชีเว็บ (WAM) เพื่อแก้ไขปัญหาการลงชื่อเข้าใช้  **หรือ** การเปิดใช้งาน ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับMicrosoft 365 Office 2013 ตรวจสอบให้แน่ใจว่าคุณเปิดใช้งานการรับรองความถูก[ต้องแบบ](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)ใหม่Officeไคลเอ็นต์ของคุณ

ดูวิธีการแก้ไขปัญหาเฉพาะที่:

[ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office 2016 รุ่น 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[คุณไม่สามารถลงชื่อเข้าใช้บัญชีขององค์กรของคุณ เช่น Office 365, Azure หรือ Intuned](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ใน Office 365, Azure หรือ Intuny](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[ได้รับพร้อมท์ซ้ําๆ เกี่ยวกับข้อมูลOffice](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)