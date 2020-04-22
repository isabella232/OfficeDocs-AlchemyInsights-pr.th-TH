---
title: การแก้ไขข้อความ บัญชีของคุณอยู่ในสถานะที่ไม่สามารถใช้งานได้ ของแอป Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547981"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>การแก้ไขข้อผิดพลาด "บัญชีของคุณอยู่ในสถานะที่ไม่สามารถใช้งานได้" ของแอป Office

ในการแก้ไขข้อผิดพลาดนี้ ให้ลองใช้ตัวเลือกต่อไปนี้กับคอมพิวเตอร์ที่ได้รับผลกระทบ:

- เปิดแอป Office เลือก **ไฟล์** > **บัญชี** > **ลงชื่อออกจากบัญชีทั้งหมด** ลงชื่อเข้าใช้อีกครั้งโดยใช้บัญชีผู้ใช้ที่มีสิทธิการใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br>
  **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity\
- หากเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Office 365 เมื่อใช้ Office 2013 [ให้เปิดใช้งานการรับรองความถูกต้องสมัยใหม่](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ Office

สำหรับข้อมูลเพิ่มเติม โปรดดู[วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ซึ่งไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

