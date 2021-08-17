---
title: การกําหนดค่าจุดสิ้นสุด DLP
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
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892818"
---
# <a name="configure-endpoint-dlp"></a>การกําหนดค่าจุดสิ้นสุด DLP

Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายการป้องกัน DLP และความสามารถในการตรวจสอบไปยังข้อมูลที่เป็นความลับWindows 10ต่างๆ หลังจากที่อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์ คุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การกระทกป้องกันบนรายการได้ สามารถใช้ Activity Explorer เพื่อตรวจสอบกิจกรรมของรายการที่ละเอียดอ่อนได้ ดูข้อมูลเพิ่มเติมได้ที่ [การออนบอร์ดอุปกรณ์ลงในการจัดการ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)อุปกรณ์  

เมื่อต้องการเริ่มต้นใช้งานจุดสิ้นสุด DLP:

- ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- ตรวจสอบสิทธิ์ที่ต้องใช้เพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์ ดูข้อมูลเพิ่มเติม [ที่](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)สิทธิ์
- อุปกรณ์ Onboard ลงในการจัดการอุปกรณ์โดยปฏิบัติตามกระบวนการอุปกรณ์ Onboarding ดูข้อมูลเพิ่มเติมได้ที่[อุปกรณ์ออนบอร์ด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) 
- สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

For more information on the Microsoft Endpoint DLP, see [learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**ขั้นตอนในการเก็บรวบรวมข้อมูลที่สําคัญ ถ้าต้องใช้การสนับสนุน:**

1. ดาวน์โหลด[ตัวอย่างตัววิเคราะห์ไคลเอ็นต์ MDATP](https://aka.ms/betamdatpanalyzer)
1. เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. เมื่อได้รับพร้อมท์ **ให้ใส่จํานวนนาทีเพื่อรวบรวมการติดตาม:** ให้ใส่จํานวนนาทีที่ต้องใช้ในการเรียกใช้สถานการณ์สมมติ
1. เรียกใช้สถานการณ์สมมติ

รวบรวมผลลัพธ์ไฟล์ Zip เพื่อให้กับตัวแทนฝ่ายสนับสนุน
