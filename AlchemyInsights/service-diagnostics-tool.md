---
title: เครื่องมือการวินิจฉัยบริการของเดสก์ท็อปเสมือนของ Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596045"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>เครื่องมือการวินิจฉัยบริการของเดสก์ท็อปเสมือนของ Windows

เดสก์ท็อปเสมือนของ Windows (WVD) มีเครื่องมือการวินิจฉัยที่ช่วยให้ผู้ดูแลระบบระบุข้อผิดพลาดผ่านทางส่วนติดต่อเดียว เครื่องมือนี้จะบันทึกข้อมูลที่เกี่ยวข้องกับการวินิจฉัยเมื่อใดก็ตามที่ WVD ถูกใช้งานโดยบุคคลที่ได้รับมอบหมายบทบาท WVD บันทึกแต่ละไฟล์จะมีข้อมูลเกี่ยวกับบทบาท WVD ที่เกี่ยวข้องกับกิจกรรม ข้อความแสดงข้อผิดพลาดที่ปรากฏระหว่างเซสชัน และข้อมูลเกี่ยวกับผู้เช่าและผู้ใช้ คุณสามารถกําหนดค่า Azure Log Analytics ให้บันทึกกิจกรรมที่สร้างขึ้นโดยเครื่องมือการวินิจฉัยโดยปฏิบัติตามขั้นตอนเหล่านี้:

1. สร้างเวิร์กสเปซ Log Analytics ด้วย[พอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2129500)หรือ[Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [เชื่อมต่อคอมพิวเตอร์ Windows กับ Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913) รับ ID เวิร์กสเปซและคีย์หลักของเวิร์กสเปซของคุณ ตัวช่วยสร้างการตั้งค่าต้องใช้ข้อมูลนี้เพื่อกําหนดค่าตัวแทนอย่างถูกต้อง และเพื่อให้แน่ใจว่าสามารถสื่อสารกับ Azure Monitor ได้

1. [ส่งข้อมูลการวินิจฉัยไปยังพื้นที่งานของคุณ](https://go.microsoft.com/fwlink/?linkid=2128284) คุณสามารถส่งข้อมูลการวินิจฉัยจากผู้เช่า WVD ของคุณไปยัง Log Analytics เพื่อเวิร์กสเปซของคุณ

1. [ระบุและวินิจฉัย](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ปัญหาภายในและภายนอกที่สัมพันธ์กับ WVD

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าเครื่องมือการวินิจฉัยบริการของ WVD ให้ดูใช้การวิเคราะห์ไฟล์บันทึกของฟีเจอร์การวินิจฉัย