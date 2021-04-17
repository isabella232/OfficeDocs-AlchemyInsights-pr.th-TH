---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833094"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>การแก้ไขข้อความ "ขออภัย บัญชีอื่นจากองค์กรของคุณลงชื่อเข้าใช้แล้ว" ของแอป Microsoft 365

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองวิธีต่อไปนี้:

- ลบบัญชีที่งานทั้งหมดออก ยกเว้นบัญชีที่ได้รับผลกระทบ โดยใช้ การตั้งค่า Windows > **Access ที่โรงเรียนหรือที่** โรงเรียน
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)
- เปิดแอป Office เลือก **บัญชี**  >  **ไฟล์**  >  **ลงชื่อออก** จากนั้นลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ที่มีสิทธิ์การใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- For Mac, [see Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

หากต้องการข้อมูลเพิ่มเติม โปรดดู["ขออภัย บัญชีอื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)