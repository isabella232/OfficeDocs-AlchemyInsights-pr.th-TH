---
title: การกําหนดค่า DLP จุดสิ้นสุด
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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402461"
---
# <a name="configure-endpoint-dlp"></a>การกําหนดค่า DLP จุดสิ้นสุด

Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายการป้องกัน DLP และความสามารถในการตรวจสอบข้อมูลที่ละเอียดอ่อนบนอุปกรณ์ Windows 10 After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items. สามารถใช้ Activity Explorer เพื่อตรวจสอบกิจกรรมของรายการที่ละเอียดอ่อนได้ ดูข้อมูลเพิ่มเติมได้ที่ [การออนบอร์ดอุปกรณ์ในการจัดการ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)อุปกรณ์  

เมื่อต้องการเริ่มต้นใช้งานจุดสิ้นสุด DLP:

- ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- ตรวจสอบสิทธิ์ที่ต้องใช้เพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าการออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์ ดูข้อมูลเพิ่มเติมได้ที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)
- อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์โดยปฏิบัติตามกระบวนการอุปกรณ์แบบออนบอร์ด ถ้าคุณไม่มีตัวเลือกการออนบอร์ดของอุปกรณ์ (ตัวอย่าง) ภายใต้การตั้งค่าการปฏิบัติตามนโยบายของ M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานและสิทธิ์ที่เหมาะสมที่อ้างอิงด้านบน ดูข้อมูลเพิ่มเติมได้ที่[อุปกรณ์การออนบอร์ด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) 
- สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**ขั้นตอนในการเก็บรวบรวมข้อมูลที่สําคัญ ถ้าต้องใช้การสนับสนุน:**

1. ดาวน์โหลดตัวอย่างตัววิเคราะห์ไคลเอ็นต์ MDATP จาก [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. เมื่อได้รับพร้อมท์ด้วย "ใส่จํานวนนาทีเพื่อรวบรวมการติดตาม: "ใส่จํานวนนาทีที่ต้องใช้เพื่อเรียกใช้สถานการณ์สมมติ
5. เรียกใช้สถานการณ์สมมติ

รวบรวมผลลัพธ์ไฟล์ Zip ที่จะให้กับตัวแทนฝ่ายสนับสนุน
