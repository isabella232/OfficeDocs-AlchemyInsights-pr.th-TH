---
title: ปัญหาในการลงชื่อเข้าใช้แอป Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763020"
---
# <a name="issues-signing-in-to-office-apps"></a>ปัญหาในการลงชื่อเข้าใช้แอป Office

เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้ด้วยแอป Office ให้ลองทําดังต่อไปนี้

- ลบบัญชีที่ทํางานทั้งหมด ยกเว้นบัญชีที่ได้รับผลกระทบ โดยใช้ การตั้งค่า Windows >**การเข้าถึงงานหรือโรงเรียน**
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \ซอฟต์แวร์\Microsoft\Office\16.0\ทั่วไป\ข้อมูลเฉพาะตัว\)
- เปิดแอป Office แล้วเลือก**ออกจากระบบบัญชี** > **Sign Out****ไฟล์** >  ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีใบอนุญาตที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- สําหรับ Mac โปรดดูที่[ไม่สามารถลงชื่อเข้าใช้แอป Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)
- ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Microsoft 365 โดยใช้ Office 2013 เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับไคลเอ็นต์ Office

สำหรับข้อมูลเพิ่มเติม ให้ดูที่
- [คุณไม่สามารถเข้าสู่ระบบ Microsoft 365, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [ปัญหาการเชื่อมต่อในการเข้าสู่ระบบหลังจากการปรับปรุง Office 2016 สร้าง 16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["ขออภัย บัญชีอื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [แก้ไขปัญหาการลงชื่อเข้าใช้ปัญหาเกี่ยวกับการรับรองความถูกต้องแบบสมัยใหม่ของ Office เมื่อคุณใช้ ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)