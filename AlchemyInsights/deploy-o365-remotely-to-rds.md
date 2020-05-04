---
title: การปรับใช้โปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรสําหรับใช้ร่วมกันบน RDS เทอร์มินัลเซิร์ฟเวอร์ หรือ VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010273"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้โปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรสําหรับใช้ร่วมกันบน RDS เทอร์มินัลเซิร์ฟเวอร์ หรือ VDI

เมื่อต้องการปรับใช้โปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:
- คุณต้องมีแผน Microsoft 365 สําหรับธุรกิจหรือแผน Office 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ E5 ขององค์กร
   > [!NOTE] 
   > แอป Microsoft 365 สําหรับธุรกิจและแผนมาตรฐานระดับพรีเมียมสําหรับธุรกิจของ Microsoft 365 ไม่รวมแอป Microsoft 365 สําหรับองค์กร
- คุณต้องเปิดใช้งาน[การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> คุณยังสามารถดาวน์โหลด และเรียกใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)การติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น คําแนะนําในการตั้งค่า และคําแนะนําในการติดตั้งแบบกําหนดเองโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่[การปรับใช้โปรแกรมประยุกต์ Microsoft 365 สําหรับองค์กร โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:
- [ดูแก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- ดู[การตั้งค่าโปรแกรมประยุกต์ของ Microsoft 365 สําหรับสถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)

ถ้าคุณต้องการติดตั้งแอป Microsoft 365 สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:

1.    ตรวจสอบสิ่งที่สมัครรับข้อมูลที่คุณมี [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
2.    หากจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
3.    ถ้า Office ได้รับการติดตั้งไว้แล้วบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft อื่นๆ ให้ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่**แผงควบคุม** > **ถอนการติดตั้งโปรแกรม** ถอนการติดตั้งโดยใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังพบปัญหา
4.    บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้ง Microsoft 365 Apps สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)
5.    หลังจากที่ติดตั้ง Office***don't open or sign in***แล้ว
6.    บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอและเลือก**Run** ในกล่อง เปิด ให้พิมพ์**regedit**แล้วเลือก**ตกลง**
   2. เลือก**ใช่**เมื่อได้รับพร้อมท์เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ
   3. ในตัวแก้ไขรีจิสทรี เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้HKEY_LOCAL_MACHINE\ซอฟต์แวร์\Microsoft \คลิกเรียกใช้\การกําหนดค่า.
   4. บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้***และ[ตรวจสอบว่า การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งานสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

