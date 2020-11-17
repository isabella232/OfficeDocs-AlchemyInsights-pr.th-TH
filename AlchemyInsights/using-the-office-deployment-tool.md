---
title: การใช้เครื่องมือการปรับใช้ Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085851"
---
# <a name="using-the-office-deployment-tool-odt"></a>การใช้เครื่องมือการปรับใช้ Office (ODT)

คุณใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อปรับใช้ office ๓๖๕เวอร์ชันของ Office เครื่องมือการปรับใช้ Office (setupodt.exe) ถูกเรียกใช้จากบรรทัดคำสั่งและใช้ไฟล์ XML การกำหนดค่าเพื่อกำหนดว่าการตั้งค่าใดที่จะนำไปใช้เมื่อปรับใช้ Office
  
1. ดาวน์โหลดเครื่องมือการปรับใช้ Office เวอร์ชันล่าสุดจาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. ใช้ [เครื่องมือกำหนดเองของ Office (OCT)](https://config.office.com) เพื่อเลือกการกำหนดลักษณะการใช้งานของคุณและสร้างไฟล์การกำหนดค่า XML ส่งออกไฟล์การกำหนดค่าและวางภายในโฟลเดอร์เดียวกันกับที่ setupodt.exe อยู่

    **หมายเหตุ:** ปัญหาการติดตั้ง Office มักเกิดขึ้นเนื่องจาก misconfigured หรือไฟล์การกำหนดค่า malformatted เมื่อต้องการหลีกเลี่ยงปัญหาดังกล่าวเราขอแนะนำให้คุณใช้เครื่องมือกำหนดเองของ Office เพื่อสร้างไฟล์การกำหนดค่า นอกจากนี้คุณยังสามารถนำเข้าไฟล์การกำหนดค่าที่มีอยู่ลงในเครื่องมือกำหนดเองของ Office ได้อีกด้วย

3. จากพร้อมท์คำสั่งยกระดับให้สลับไปยังตำแหน่งที่ตั้งที่ setupodt.exe อยู่และเรียกใช้เครื่องมือการปรับใช้ Office ในโหมดดาวน์โหลดและระบุไฟล์การกำหนดค่าที่คุณเพิ่งบันทึก ในตัวอย่างนี้ไฟล์การกำหนดค่าจะถูกตั้งชื่อ Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. เรียกใช้เครื่องมือการปรับใช้ Office ในโหมดกำหนดค่าและระบุไฟล์การกำหนดค่า

```setupodt.exe /configure Configuration.xml```

**หมายเหตุ:** คุณต้องเรียกใช้ขั้นตอนนี้จากคอมพิวเตอร์ไคลเอ็นต์ที่คุณต้องการติดตั้ง Office และคุณต้องมีสิทธิ์ของผู้ดูแลระบบภายในบนคอมพิวเตอร์เครื่องนั้น

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการใช้เครื่องมือการปรับใช้ Office สำหรับสถานการณ์การปรับใช้ Microsoft ๓๖๕สำหรับองค์กรของคุณให้ดู[ที่ภาพรวมของเครื่องมือการปรับใช้ office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีใช้เครื่องมือกำหนดเองของ Office ให้ดูที่[ภาพรวมของเครื่องมือกำหนดเองของ office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
