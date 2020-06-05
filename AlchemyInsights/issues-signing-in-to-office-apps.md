---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579956"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>การแก้ไขแอป Microsoft 365 "ขออภัย บัญชีอื่นจากองค์กรของคุณลงชื่อเข้าใช้แล้ว"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองทําดังต่อไปนี้

- เอาบัญชีงานทั้งหมดออก ยกเว้นบัญชีที่ได้รับผลกระทบ โดยใช้การตั้งค่า Windows > **Access งานหรือโรงเรียน**
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \ซอฟต์แวร์\Microsoft\Office\16.0\ทั่วไป\รหัสประจําตัว\)
- เปิดแอป Office เลือก**การ**  >  **Account**  >  **ลงชื่อออก**บัญชีไฟล์ จากนั้นลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ที่มีสิทธิ์การใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- สําหรับ Mac ให้ดูที่[ไม่สามารถลงชื่อเข้าใช้แอป Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)ได้

สําหรับข้อมูลเพิ่มเติม ให้ดูที่["ขออภัย บัญชีอื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)