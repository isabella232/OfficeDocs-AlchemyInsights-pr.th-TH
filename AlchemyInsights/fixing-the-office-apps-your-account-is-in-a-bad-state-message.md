---
title: การแก้ไขแอป Office บัญชีของคุณอยู่ในข้อความสถานะไม่ถูกต้อง
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969869"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>การแก้ไขแอปพลิเคชัน Office "บัญชีของคุณอยู่ในสถานะที่ไม่ดี"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองใช้ตัวเลือกต่อไปนี้บนคอมพิวเตอร์ที่ได้รับผลกระทบ:

- เปิดแอป Office เลือก**บัญชี** > **ไฟล์** > **ลงชื่อออกจากบัญชีทั้งหมด** เข้าสู่ระบบอีกครั้งโดยใช้บัญชีผู้ใช้ที่มีใบอนุญาตที่ถูกต้อง สำหรับข้อมูลเพิ่มเติมโปรดดู[ที่บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br>
  **หมายเหตุ:** เส้นทางรีจิสทรีสำหรับ Office ๒๐๑๖มีการเปลี่ยนแปลงเป็น๑๖.๐ ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity\
- บนคอมพิวเตอร์ที่ได้รับผลกระทบตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:  
     1. คลิกขวาที่ปุ่ม Windows และเลือก**Run** ในกล่อง**เปิด**พิมพ์**Regedit**แล้วเลือก**ตกลง**
     2. เลือก**ใช่**เมื่อได้รับพร้อมท์เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ
    3. ในตัวแก้ไขรีจิสทรีให้เพิ่มค่า DWORD ของ EnableADAL ด้วยการตั้งค่า0ภายใต้ HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- ถ้ามีข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Office ๓๖๕ใช้ Office ๒๐๑๓[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ของ Office

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการแก้ปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถเข้าสู่ระบบ Office ๓๖๕, Azure หรือ Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

