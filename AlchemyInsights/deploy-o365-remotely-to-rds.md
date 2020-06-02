---
title: การปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรสําหรับการใช้งานที่ใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัล หรือ VDI
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507605"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรสําหรับการใช้งานที่ใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัล หรือ VDI

เมื่อต้องการปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล (RDS), ชื่อเดิมคือบริการเทอร์มินัล:
- คุณต้องมีแผน Microsoft 365 สําหรับธุรกิจหรือแผน Office 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ Enterprise E5
   > [!NOTE] 
   > แอป Microsoft 365 สําหรับธุรกิจและแผนมาตรฐานพรีเมี่ยมสําหรับธุรกิจ Microsoft 365 ไม่รวมแอป Microsoft 365 สําหรับองค์กร
- คุณต้องเปิดใช้งาน[การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> คุณยังสามารถดาวน์โหลด และเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น[Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:
- ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- ดู[รีเซ็ตแอป Microsoft 365 สําหรับสถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)

ถ้าคุณต้องการติดตั้ง Microsoft 365 Apps สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:

1.    ตรวจสอบสิ่งที่คุณมีการสมัครใช้งาน [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2.    หากจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3.    ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft อื่น ๆ ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่**แผงควบคุม**  >  **การถอนการติดตั้งโปรแกรม** ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังทํางานเป็นปัญหา
4.    บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้งแอป Microsoft 365 สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)
5.    หลังจากที่มีการติดตั้ง Office***แล้ว***
6.    บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอแล้วเลือก**เรียกใช้** ในกล่อง เปิด ให้พิมพ์**regedit**แล้วเลือก**ตกลง**
   2. เลือก**ใช่**เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ
   3. ในตัวแก้ไขรีจิสทรี ให้เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\คลิกToRun\การกําหนดค่า
   4. บนเซิร์ฟเวอร์ RDS***ให้ลงชื่อเข้าใช้ในฐานะผู้ใช้ และ***[ตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

