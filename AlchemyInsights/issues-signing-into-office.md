---
title: ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938366"
---
# <a name="issues-signing-in-to-office-apps"></a>ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office

เมื่อต้องการแก้ไขปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ Office ลองต่อไปนี้:

- เอาบัญชีงานทั้งหมด ยกเว้นบัญชีได้รับผลกระทบ โดยใช้การตั้งค่า Windows >**เข้างานหรือที่โรงเรียน**
- [ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0 (แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)
- เปิดโปรแกรมประยุกต์ Office เลือก**แฟ้ม** > **บัญชี** > **เครื่องหมายออก** จากนั้น เข้าสู่ระบบโดยใช้บัญชีผู้ใช้ที่มีลิขสิทธิ์ถูกต้อง สำหรับข้อมูลเพิ่มเติม ให้ดู[บัญชีผู้ใช้ใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- สำหรับ Mac ดู[ไม่สามารถเข้าสู่ระบบเป็น 2016 Office สำหรับแอพลิเคชัน Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)
- ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับโดยใช้ Office 2013 Office 365 เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับไคลเอ็นต์ของ Office

สำหรับข้อมูลเพิ่มเติม ให้ดูที่
- [คุณไม่สามารถเข้าสู่ระบบ Office 365, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [ปัญหาการเชื่อมต่อในเครื่องหลังจากการปรับปรุง Office 2016 16.0.7967 ที่สร้างบน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["ขอโทษ บัญชีผู้ใช้อื่นจากองค์กรของคุณมีอยู่แล้วลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [การแก้ไขปัญหาการเข้าสู่ระบบปัญหาเกี่ยวกับการรับรองความถูกต้องแบบสมัยใหม่ของ Office เมื่อคุณใช้ ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)