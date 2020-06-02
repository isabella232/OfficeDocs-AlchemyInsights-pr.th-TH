---
title: การติดตั้งสํานักงานบนเซิร์ฟเวอร์เทอร์มินัล - ไม่มีสิทธิ์การใช้งาน
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508647"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล

สําหรับการปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรบนเซิร์ฟเวอร์ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), ชื่อเดิมคือบริการเทอร์มินัล:
  
- คุณต้องมีการสมัครใช้งาน Microsoft 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ Enterprise E5 แอป Microsoft 365 สําหรับธุรกิจและ Microsoft 365 Apps สําหรับธุรกิจแผนพรีเมี่ยมไม่รวมแอป Microsoft 365 สําหรับองค์กร

- คุณต้องเปิดใช้งาน[คอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

ถ้าคุณต้องการติดตั้ง Microsoft 365 Apps สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้

> [!TIP]
> คุณยังสามารถดาวน์โหลด และเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน
  
1. ตรวจสอบว่าการสมัครใช้งาน Microsoft 365 ที่คุณมี [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งาน Microsoft 365 อื่น [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft 365 อื่น ๆ ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่แผงควบคุม \> การถอนการติดตั้งโปรแกรม ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังทํางานเป็นปัญหา

4. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้งแอป Microsoft 365 สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากที่มีการติดตั้ง Office***แล้ว***

6. บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:

1. คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอแล้วเลือก เรียกใช้ ในการOPENกล่อง ชนิด**regedit,** แล้ว เลือกตกลง.

2. เลือก ใช่ เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ

3. ในตัวแก้ไขรีจิสทรี ให้เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\คลิกToRun\การกําหนดค่า

7. บนเซิร์ฟเวอร์ RDS***ให้ลงชื่อเข้าใช้ในฐานะผู้ใช้ และ***[ตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น[Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โปรดดู[การแก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  