---
title: ปัญหาในการลงชื่อเข้าใช้Microsoft 365แอป
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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028059"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>การแก้ไขปัญหาแอปMicrosoft 365 "ขออภัย บัญชีอื่นจากองค์กรของคุณลงชื่อเข้าใช้แล้ว"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองวิธีต่อไปนี้:

- เอาบัญชีที่งานทั้งหมดออก ยกเว้นบัญชีที่ได้รับผลกระทบ โดยใช้ Windows การตั้งค่า > **Access ที่โรงเรียนหรือที่** โรงเรียน
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)
- เปิดไฟล์แอป Office บัญชี  >  **ไฟล์**  >  **ลงชื่อ** ออก จากนั้นลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ที่มีสิทธิ์การใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

ดูข้อมูลเพิ่มเติมที่["ขออภัย บัญชีอื่นจากองค์กรของคุณลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)