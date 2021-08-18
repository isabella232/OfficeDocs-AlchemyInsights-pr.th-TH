---
title: ตัวบ่งชี้ไม่ใช้งานโดยใช้เบราว์เซอร์ Microsoft Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326280"
---
# <a name="indicators-dont-work-using-edge-browser"></a>ตัวบ่งชี้ไม่ใช้งานโดยใช้เบราว์เซอร์ Microsoft Edge

หลังจากที่คุณสร้างตัวบ่งชี้ Edge (SmartScreen) จะไม่แสดงขึ้น For more information, see [Create indicators for IPs and URLs/domains](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>ขั้นตอนที่ 1: ตรวจสอบให้แน่ใจว่า

- ตรวจสอบว่าตัวบ่งชี้ถูกต้อง (ไม่มีการพิมพ์ผิดใน IP/URL การปฏิบัติการที่ถูกต้อง กลุ่ม RBAC ที่ถูกต้อง)
- รออย่างน้อย 2 ชั่วโมงหลังจากสร้างตัวบ่งชี้เพื่อใช้เวลาในการเวลาแฝงที่เป็นไปได้
- ยืนยันว่าระบบออนบอร์ดกับ Microsoft Defender for Endpoint
- ตรวจสอบว่าระบบนั้นสามารถสื่อสารกับระบบคลาวด์ได้
- ตรวจสอบว่า SmartScreen เปิดใช้งานและเข้าถึงได้โดย [ไปที่ไซต์](https://demo.smartscreen.msft.net)ทดสอบ

## <a name="step-2-troubleshoot-the-potential-issue"></a>ขั้นตอนที่ 2: แก้ไขปัญหาที่อาจเกิดขึ้น

- ตรวจสอบให้แน่ใจว่าไคลเอ็นต์ตรงตามความต้องการ For details, see [Create indicators for IPs and URLs/domains](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- ตรวจสอบให้แน่ใจว่าคุณใช้เบราว์เซอร์ Microsoft Edge เวอร์ชันล่าสุด เมื่อต้องการค้นหาเวอร์ชันล่าสุด ให้ดู[ค้นหาเวอร์ชันMicrosoft Edgeเวอร์ชัน](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)ที่คุณมี
- รีสตาร์ตเบราว์เซอร์ Microsoft Edge
- นําทางไปยังไซต์ที่คุณได้ตั้งค่าตัวบ่งชี้ไว้ ถ้าไซต์ไม่ปรากฏตามที่คาดไว้ ให้ไปยังขั้นตอนที่ 3 

## <a name="step-3-collect-data"></a>ขั้นตอนที่ 3: รวบรวมข้อมูล

- รวบรวมข้อมูล **การวินิจฉัย MDEClientAnalyzer** ดูคําแนะ[นําที่ ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoint](issues-with-onboarding-machines.md)
- ถ้าคุณคุ้นเคยกับการติดตั้งและการรวบรวมการติดตาม Fiddler ให้ดู[Telerik Fiddler](http://www.telerik.com/fiddler)
- ถ้าคุณต้องการแนวทางจากฝ่ายสนับสนุนของ Microsoft ให้เลือกไอคอน การสนับสนุน ทางด้านล่างเพื่อเปิดกรณีการสนับสนุน
