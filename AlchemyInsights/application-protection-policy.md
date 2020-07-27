---
title: นโยบายการป้องกันแอปพลิเคชัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423958"
---
# <a name="application-protection-policy"></a>นโยบายการป้องกันแอปพลิเคชัน

หากคุณเพิ่งเริ่มใช้นโยบายการป้องกันแอปพลิเคชัน (APP) โปรดดู[ภาพรวมนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/apps/app-protection-policy)

เมื่อต้องการเริ่มใช้ APP ให้ดูที่[วิธีสร้างและกําหนดนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies)

ข้อกําหนดนโยบายการป้องกันแอปพลิเคชัน:

- ผู้ใช้มีสิทธิ์การใช้งาน Intun หรือ EMS
- ผู้ใช้เป็นสมาชิกของกลุ่มที่กําหนดเป้าหมายตามนโยบายการป้องกันแอปพลิเคชัน
- ผู้ใช้ขององค์กรเพียงคนเดียวเท่านั้นที่ลงชื่อเข้าใช้แอปที่มีการป้องกันบนอุปกรณ์
- โปรแกรมประยุกต์ได้ดําเนินการ[ใน Intunเย SDK](https://docs.microsoft.com/intune/app-sdk-get-started) สําหรับรายการแอปที่สนับสนุน SDK โปรดดู[แอปที่มีการป้องกันของ Microsoft Intun](https://docs.microsoft.com/intune/apps-supported-intune-apps)

นโยบายจะนําไปใช้หลังจากผู้ใช้ที่มีคุณสมบัติตรงตามข้อกําหนดข้างต้นที่ลงชื่อเข้าใช้แอปที่เปิดใช้งาน Intuner SDK วิธีที่ง่ายที่สุดในการตรวจสอบว่ามีการใช้นโยบายหรือไม่ 

สำหรับข้อมูลเพิ่มเติม ให้ดูที่

[คําถามที่พบบ่อยเกี่ยวกับการแก้ไขปัญหาของ APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[วิธีตรวจสอบการตั้งค่านโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies-validate)

[ทําความเข้าใจเกี่ยวกับระยะเวลาในการส่งนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[วิธีตรวจสอบนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies-monitor)