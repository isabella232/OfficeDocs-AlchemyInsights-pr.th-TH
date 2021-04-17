---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815634"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intun1

นโยบายการป้องกันปลายทางของ Intunes สามารถใช้เพื่อกําหนดค่าการตั้งค่าการเข้ารหัสลับ Bitlocker บนอุปกรณ์ Windows หากต้องการข้อมูลเพิ่มเติม โปรดดูการตั้งค่า[Windows 10 (และใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intun1](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

นอกจากนโยบายการป้องกันจุดสิ้นสุดแล้ว ยังมีรายงานการเข้ารหัสลับซึ่งให้มุมมองโดยละเอียดมากขึ้นของสถานะการเข้ารหัสลับของอุปกรณ์ รายงานนี้สามารถเข้าถึงได้จากพอร์ทัล MEM ภายใต้ **อุปกรณ์ > Monitor** จากนั้น ภายใต้ การกําหนด **ค่า** ให้เลือก [รายงาน](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)การเข้ารหัสลับ

ถ้าคุณพบว่า Bitlocker ไม่สามารถเปิดใช้งานตามที่คาดไว้หรือโปรไฟล์ที่ใช้เพื่อเปิดใช้งาน Bitlocker อยู่ในสถานะข้อผิดพลาด โปรดตรวจสอบรายงานการเข้ารหัสลับเพื่อให้เข้าใจสาเหตุที่ลักษณะการเกิดขึ้นได้ดีขึ้น

เมื่อต้องการค้นหารายละเอียดเกี่ยวกับวิธีการแปลรายงานรวมถึงค่าสถานะการเข้ารหัสลับต่างๆ ให้ดู[ตรวจสอบการเข้ารหัสลับอุปกรณ์ด้วย Intunes](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

คุณควรทราบว่าอุปกรณ์ที่ใหม่กว่าหลายเครื่องที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับ Bitlocker โดยอัตโนมัติ ซึ่งจะถูกทริกเกอร์โดยไม่มีแอปพลิเคชันนโยบาย MDM ซึ่งอาจส่งผลกระทบต่อการใช้นโยบายถ้ามีการกําหนดค่าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้น ดู FAQ ต่อไปนี้เพื่อดูรายละเอียดเพิ่มเติม

For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies intun1](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**คำถามที่ถามบ่อย**

Q: Windows รุ่นใดที่สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันจุดสิ้นสุด<br>
A: การตั้งค่าใน นโยบายการป้องกันจุดสิ้นสุดของ Intuned จะถูกปรับใช้โดยใช้[Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Windows ไม่รองรับ Bitlocker CSP ทุกรุ่นหรือทุกรุ่น <br><br>

Q: Bitlocker สามารถเปิดใช้งานบนอุปกรณ์โดยไม่ต้องมีการโต้ตอบของผู้ใช้ได้อย่างไร<br>
A: ถ้าตรงตามเงื่อนไขที่จําเป็นแล้วคุณจึงสามารถเปิดใช้งาน Bitlocker "Silent Encryption" ผ่าน Intunes ได้ ดูรายละเอียดของความต้องการของอุปกรณ์และการตั้งค่านโยบายตัวอย่างเพื่อเปิดใช้งานการเข้ารหัสลับแบบไม่ระบุข้อมูลในเอกสารต่อไปนี้: [เปิดใช้งานการเข้ารหัสลับ Bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)โดยไม่เปิด <br><br>

Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของ OS ในวิธีการเข้ารหัสลับและจุดแข็งการเข้ารหัส (XTS-AES-128) จะปรับใช้นโยบายที่มีการตั้งค่าอื่นทริกเกอร์การเข้ารหัสลับไดรฟ์ใหม่ด้วยการตั้งค่าใหม่โดยอัตโนมัติหรือไม่<br>
A: ไม่ได้ เมื่อต้องการใช้การตั้งค่าการเข้ารหัสใหม่ ไดรฟ์จะต้องถูกถอดรหัสลับก่อน<br><br>
**หมายเหตุ:** For devices being enrolled with Autopilot, the automatic encryption that would would occur during OOBE is not triggered until Intuned policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.
 
Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลจากแอปพลิเคชันนโยบาย Intuned อุปกรณ์จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่<br>
A: การเอานโยบายที่เกี่ยวข้องกับการเข้ารหัสลับออกไม่ส่งผลให้มีการเข้ารหัสลับไดรฟ์ที่ถูกกําหนดค่า
 
Q: เหตุใดนโยบายการปฏิบัติตามนโยบาย Intun1 จึงแสดงให้เห็นว่าอุปกรณ์ของฉันไม่เปิดใช้งาน Bitlocker แม้ว่าจะเป็นเพราะอะไร<br>
A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบาย Intun <2> ใช้ไคลเอ็นต์การทดสอบสถานภาพของอุปกรณ์ Windows (DHA) ไคลเอ็นต์นี้วัดสถานะอุปกรณ์เมื่อเริ่มระบบเท่านั้น ดังนั้นถ้ายังไม่ได้เริ่มต้นระบบใหม่เนื่องจากการเข้ารหัสลับ Bitlocker เสร็จสมบูรณ์แล้ว บริการไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ว่าใช้งานอยู่
 
 