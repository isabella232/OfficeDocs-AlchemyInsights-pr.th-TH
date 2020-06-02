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
ms.openlocfilehash: 5592158c24ae55d712018d6886670fe8e9a794c3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44499242"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>การแก้ไขข้อผิดพลาด "บัญชีของคุณอยู่ในสถานะที่ไม่สามารถใช้งานได้" ของแอป Office

ในการแก้ไขข้อผิดพลาดนี้ ให้ลองใช้ตัวเลือกต่อไปนี้กับคอมพิวเตอร์ที่ได้รับผลกระทบ:

- เปิดแอป Office เลือก **ไฟล์** > **บัญชี** > **ลงชื่อออกจากบัญชีทั้งหมด** ลงชื่อเข้าใช้อีกครั้งโดยใช้บัญชีผู้ใช้ที่มีสิทธิการใช้งานที่ถูกต้อง สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br>
  **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity\
- หากเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Office 365 เมื่อใช้ Office 2013 [ให้เปิดใช้งานการรับรองความถูกต้องสมัยใหม่](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ Office

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีการแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Microsoft 365, Azure หรือ Intun](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

