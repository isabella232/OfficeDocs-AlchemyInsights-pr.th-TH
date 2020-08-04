---
title: ตั้งค่าคอนฟิก DLP ปลายทาง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556033"
---
# <a name="configure-endpoint-dlp"></a>ตั้งค่าคอนฟิก DLP ปลายทาง

Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายความสามารถในการป้องกันและการตรวจสอบ DLP ไปยังข้อมูลที่ละเอียดอ่อนบนอุปกรณ์ Windows 10 หลังจากที่อุปกรณ์ถูกเปิดใช้งานในการจัดการอุปกรณ์แล้ว คุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การดําเนินการป้องกันบนรายการได้ ตัวสํารวจกิจกรรมสามารถใช้ในการตรวจสอบกิจกรรมสําหรับรายการที่สําคัญ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเตรียมพร้อมอุปกรณ์เข้าสู่การจัดการอุปกรณ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)  

เมื่อต้องการเริ่มต้นใช้งานปลายทาง DLP:

- ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การออกใบอนุญาต SKU/การสมัครใช้งาน](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)
- ตรวจสอบสิทธิ์ที่จําเป็นเพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)
- อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์โดยทําตามขั้นตอนอุปกรณ์ออนบอร์ด หากคุณไม่มีตัวเลือกการเตรียมพร้อมสําหรับอุปกรณ์ (ดูตัวอย่าง) ภายใต้**การตั้งค่า**การปฏิบัติตามข้อกําหนด M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานและสิทธิ์ที่เหมาะสมที่อ้างอิงข้างต้น สําหรับข้อมูลเพิ่มเติม ให้ดูที่[อุปกรณ์ออนบอร์ด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) 
- สร้างนโยบาย DLP เพื่อปกป้องรายการที่ละเอียดอ่อนของคุณ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สถานการณ์จําลองนโยบาย DLP ปลายทาง](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับ Microsoft ปลายทาง DLP ดู[เรียนรู้เกี่ยวกับ Microsoft 365 ปลายทางข้อมูลสูญหายป้องกัน (ตัวอย่าง)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)