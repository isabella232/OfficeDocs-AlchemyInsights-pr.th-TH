---
title: การติดตั้งสํานักงานบนเซิร์ฟเวอร์เทอร์มินัล - ไม่มีใบอนุญาต
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763236"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล

สําหรับการปรับใช้โปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรบนเซิร์ฟเวอร์ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:
  
- คุณต้องมีการสมัครใช้งาน Microsoft 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ E5 สําหรับองค์กร แอป Microsoft 365 สําหรับธุรกิจและแอป Microsoft 365 สําหรับธุรกิจแบบพรีเมียมไม่มีแอป Microsoft 365 สําหรับองค์กร

- คุณต้องเปิดใช้งาน[การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

ถ้าคุณต้องการติดตั้งแอป Microsoft 365 สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้

> [!TIP]
> คุณยังสามารถดาวน์โหลด และเรียกใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)การติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน
  
1. ตรวจสอบการสมัครใช้งาน Microsoft 365 ที่คุณมี [เรียนรู้วิธีการ](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งาน Microsoft 365 อื่น [เรียนรู้วิธีการ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. ถ้า Office ได้รับการติดตั้งไว้แล้วบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft 365 อื่นๆ ให้ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่แผงควบคุม\>ถอนการติดตั้งโปรแกรม ถอนการติดตั้งโดยใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังพบปัญหา

4. บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้ง Microsoft 365 Apps สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากที่ติดตั้ง Office***don't open or sign in***แล้ว

6. บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:

1. คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอและเลือก ในกล่อง เปิด ให้พิมพ์**regedit**แล้วเลือก ตกลง

2. เลือก ใช่ เมื่อได้รับพร้อมท์เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ

3. ในตัวแก้ไขรีจิสทรี เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้HKEY_LOCAL_MACHINE\ซอฟต์แวร์\Microsoft \คลิกเรียกใช้\การกําหนดค่า.

7. บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้***และ[ตรวจสอบว่า การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งานสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น[Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)
  
เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สําหรับ Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  