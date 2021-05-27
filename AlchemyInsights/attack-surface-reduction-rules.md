---
title: กฎการลดพื้นหน้าของการโจมตี
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676445"
---
# <a name="attack-surface-reduction-rules"></a>กฎการลดพื้นหน้าของการโจมตี

การยกเว้นไฟล์หรือโฟลเดอร์อาจลดการป้องกันอย่างร้ายแรงจากกฎการลดพื้นหน้าของการโจมตีได้ ไฟล์ที่ถูกบล็อกโดยกฎจะได้รับอนุญาตให้เรียกใช้ และจะไม่มีบันทึกรายงานหรือเหตุการณ์ การยกเว้นจะใช้กับกฎทั้งหมดที่อนุญาตให้ยกเว้นได้

การยกเว้น ASR จะใช้ไวยากรณ์เดียวกับโปรแกรมป้องกันไวรัสของ Microsoft Defenderแยกออก For details, see [Configure and validate exclusions for โปรแกรมป้องกันไวรัสของ Microsoft Defender scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). เพื่อหลีกเลี่ยงปัญหา ให้ตรวจดู[ข้อผิดพลาดทั่วไปเพื่อหลีกเลี่ยงเมื่อระบุข้อยกเว้น](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

กฎ ASR บางรายการไม่สนับสนุนข้อยกเว้น เมื่อต้องการตรวจสอบว่ากฎของคุณสนับสนุนข้อยกเว้นหรือไม่ ให้ดูตาราง กฎ [การลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)การโจมตี

## <a name="attack-surface-reduction-rules"></a>กฎการลดพื้นหน้าของการโจมตี

พื้นหน้าการโจมตีขององค์กรของคุณรวมสถานที่ที่ผู้โจมตีอาจโจมตีอุปกรณ์หรือเครือข่ายขององค์กรได้ การลดพื้นหน้าของการโจมตีของคุณหมายถึงการปกป้องอุปกรณ์ขององค์กรและเครือข่าย ซึ่งทิ้งให้ผู้โจมตีมีวิธีการโจมตีลดลง การกําหนดค่ากฎการลดพื้นหน้าของการโจมตีใน Microsoft Defender for Endpoint สามารถช่วยได้

สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [แมป GUID ของกฎ ASR กับชื่อ](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ความต้องการของกฎ ASR:
    - [Windows 10 Pro เวอร์ชัน 1709 หรือใหม่กว่า](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise เวอร์ชัน 1709 หรือใหม่กว่า](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows เซิร์ฟเวอร์ เวอร์ชัน 1803 (แชนเนลรายครึ่งปี) หรือใหม่กว่า](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>ระบุการยกเว้นที่ถูกต้องที่จะปรับใช้

1. ค้นหา eventID 1121 หรือ 1122 ใน Microsoft-Windows-Windows Defender/บันทึกการปฏิบัติการ

1. ประเมินสถานการณ์การบล็อกและบริบท และยืนยันว่าสถานการณ์นี้ต้องไม่ถูกบล็อก

1. อ่านค่า เส้นทาง ในรายละเอียดเหตุการณ์ ซึ่งเป็นค่าที่กําหนดการยกเว้น
    - ให้ข้อยกเว้นเคร่งครัดที่สุดเท่าที่จะเป็นไปได้
    - ใช้อักขระตัวแทนที่ต้องการ (ตัวอย่างเช่น แทนที่ตัวแปรผู้ใช้)

1. ปรับใช้ข้อยกเว้นตามความต้องการในการปรับใช้ของคุณ โปรดดูรายละเอียดที่ ปรับแต่ง [กฎการลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)การโจมตี

## <a name="exclusion-is-not-honored"></a>ไม่รับการยกเว้น

1. ระบุว่ากฎสนับสนุนข้อยกเว้นหรือไม่ ดูรายละเอียดที่ [กฎการลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)การโจมตี

1. ตรวจทานข้อยกเว้นที่ปรับใช้และตรวจสอบด้วยข้อมูลเหตุการณ์ของอักขระตัวแทนที่พิมพ์ผิดหรือมีแปลผิด หากต้องการข้อมูลเพิ่มเติม โปรดดูประเภท [การยกเว้นที่ได้รับการสนับสนุน](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ถ้าผลกระทบของกฎสูงเกินไป ให้พิจารณาย้ายกฎ (ย้อนกลับ) ไปยังโหมดตรวจสอบเพื่อการตรวจสอบความถูกต้องเพิ่มเติม ดูรายละเอียดที่ [ทดสอบวิธีที่คุณลักษณะของ Microsoft Defender for Endpoint สามารถใช้งานในโหมด](/microsoft-365/security/defender-endpoint/audit-windows-defender)ตรวจสอบ

1. รวบรวมข้อมูลการสนับสนุนเพื่อเปิดกรณีสนับสนุนโดยใช้การสั่งนี้:
    
   ** MDEClientAnalyzer.cmd -v**

    For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).
