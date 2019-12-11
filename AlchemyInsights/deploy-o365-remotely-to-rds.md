---
title: การจัดวาง Office ๓๖๕ ProPlus สำหรับใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัลหรือ VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959478"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>การจัดวาง Office ๓๖๕ ProPlus สำหรับใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัลหรือ VDI

เพื่อปรับใช้ Office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:
- คุณต้องมี Microsoft ๓๖๕สำหรับแผนธุรกิจหรือแผน Office ๓๖๕ที่รวม Office ๓๖๕ ProPlus เช่น Office ๓๖๕เอ็นเตอร์ไพรส์ E3 หรือองค์กร E5
   > [!NOTE] 
   > แผนพรีเมียม Office ๓๖๕ธุรกิจและ Office ๓๖๕ไม่รวม Office ๓๖๕ ProPlus
- คุณต้องเปิดการใช้[งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

> [!NOTE]
> นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Office ๓๖๕ ProPlus ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำในการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่การจัดวาง[office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)

วิธีแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:
- ดู[การแก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
- ดูที่การ[ตั้งค่าสถานะการเปิดใช้งาน Office ๓๖๕ ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218)

ถ้าคุณต้องการติดตั้ง Office ๓๖๕ ProPlus บน RDS จากศูนย์ดูแล Microsoft ๓๖๕***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:

1.  ตรวจสอบว่าคุณมีแผน Office ๓๖๕ใดบ้าง [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)การ
2.  ถ้าจำเป็นให้สลับไปยังแผน Office ๓๖๕อื่น [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)การ
3.  ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office ๓๖๕อื่นๆที่มีอยู่ให้ถอนการติดตั้ง ตัวอย่างเช่นโดยไปที่**แผง** > ควบคุม**ถอนการติดตั้งโปรแกรม** ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังทำงานเป็นปัญหา
4.  บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์ดูแลของ Microsoft ๓๖๕กับบัญชีผู้ดูแลระบบของคุณและ[ติดตั้ง Office ๓๖๕ ProPlus](https://portal.office.com/OLS/MySoftware.aspx)
5.  หลังจากติดตั้ง Office แล้ว***อย่าเปิดหรือลงชื่อเข้า***ใช้โปรแกรมประยุกต์ office ใดๆ
6.  บนเซิร์ฟเวอร์ RDS เปิดการใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอของคุณและเลือก**เรียกใช้** ในกล่องเปิดพิมพ์**regedit**และจากนั้นให้เลือก **' ตกลง '**
   2. เลือก**ใช่**เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทำการเปลี่ยนแปลงอุปกรณ์ของคุณ
   3. ในตัวแก้ไขรีจิสทรีเพิ่มค่าสตริงของการอนุญาตให้ใช้**สิทธิ์ Sharedคอมพิวเตอร์**ที่มีการตั้งค่าของ1ภายใต้ HKEY_LOCAL_MACHINE \ ซอฟต์แวร์ \ Microsoft \Office\ClickToRun\Configuration.
   4. บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้ปลาย***ทางและตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้[ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

