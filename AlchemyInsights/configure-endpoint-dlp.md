---
title: กำหนดค่าจุดสิ้นสุด DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305462"
---
# <a name="configure-endpoint-dlp"></a>กำหนดค่าจุดสิ้นสุด DLP

Microsoft จุดสิ้นสุด DLP ช่วยให้คุณสามารถขยายความสามารถในการป้องกัน DLP และการตรวจสอบความสามารถของข้อมูลที่สำคัญบนอุปกรณ์ Windows 10 หลังจากที่อุปกรณ์ onboarded เข้าสู่การจัดการอุปกรณ์แล้วคุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การดำเนินการป้องกันในรายการได้ กิจกรรม Explorer สามารถใช้เพื่อตรวจสอบกิจกรรมสำหรับรายการที่มีความสำคัญได้ สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศลงในการจัดการอุปกรณ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)  

เมื่อต้องการเริ่มต้นใช้งาน DLP สำหรับจุดสิ้นสุดให้ทำดังนี้

- ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม สำหรับข้อมูลเพิ่มเติมให้ดูที่สิทธิ์การใช้งาน [SKU/การสมัคร](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)ใช้งาน
- ตรวจสอบสิทธิ์ที่จำเป็นในการเปิดใช้งานการจัดการอุปกรณ์ให้เข้าถึงหน้าปฐมนิเทศหรือเปิด/ปิดการตรวจสอบอุปกรณ์ สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)
- อุปกรณ์ Onboard ลงในการจัดการอุปกรณ์โดยการติดตามขั้นตอนอุปกรณ์ปฐมนิเทศ ถ้าคุณไม่พบตัวเลือกอุปกรณ์ปฐมนิเทศ (preview) ภายใต้  **การตั้งค่าการ**ปฏิบัติตามข้อบังคับ M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานที่เหมาะสมและสิทธิ์ที่อ้างอิงด้านบน สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) 
- สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ สำหรับข้อมูลเพิ่มเติมให้ดูที่ [สถานการณ์สมมติของนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)ของจุดสิ้นสุด

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ DLP จุดสิ้นสุดของ Microsoft ให้ดูที่[เรียนรู้เกี่ยวกับการป้องกันการสูญหายของข้อมูลจุดสิ้นสุดของ microsoft ๓๖๕ (การแสดงตัวอย่าง)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)

**ขั้นตอนการรวบรวมข้อมูลที่สำคัญถ้าจำเป็นต้องมีการสนับสนุน:**

1. ดาวน์โหลด MDATP การแสดงตัวอย่างตัววิเคราะห์ไคลเอ็นต์จาก [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")
2. เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd – t
4. เมื่อได้รับพร้อมท์ด้วย "ใส่จำนวนนาทีในการรวบรวมการสืบค้นกลับ:" ให้ใส่จำนวนนาทีที่จำเป็นต้องใช้ในการเรียกใช้สถานการณ์สมมติ
5. เรียกใช้สถานการณ์สมมติ

การรวบรวมผลลัพธ์ของไฟล์ Zip ที่จะมอบให้กับตัวแทนฝ่ายสนับสนุน
