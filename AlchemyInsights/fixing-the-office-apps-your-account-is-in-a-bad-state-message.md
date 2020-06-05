---
title: การแก้ไขแอป Microsoft 365 บัญชีของคุณอยู่ในข้อความสถานะที่ไม่ถูกต้อง
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
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580136"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>การแก้ไขข้อผิดพลาดในแอป Microsoft 365 "บัญชีของคุณอยู่ในสถานะไม่ถูกต้อง"

ในการแก้ไขข้อผิดพลาดนี้ ให้ลองใช้ตัวเลือกต่อไปนี้กับคอมพิวเตอร์ที่ได้รับผลกระทบ:

- เปิดแอป Office เลือก **ไฟล์** > **บัญชี** > **ลงชื่อออกจากบัญชีทั้งหมด** ลงชื่อเข้าใช้อีกครั้งโดยใช้บัญชีผู้ใช้ที่มีสิทธิการใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br>
  **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity\
- หากเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Office 365 เมื่อใช้ Office 2013 [ให้เปิดใช้งานการรับรองความถูกต้องสมัยใหม่](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ Office

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีการแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Microsoft 365, Azure หรือ Intun](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

