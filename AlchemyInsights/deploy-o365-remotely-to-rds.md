---
title: การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรสำหรับการใช้งานร่วมกันบน RDS, Terminal Server หรือ VDI
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786296"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรสำหรับการใช้งานร่วมกันบน RDS, Terminal Server หรือ VDI

เมื่อต้องการปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรที่ใช้บริการเดสก์ท็อประยะไกล (RDS) ซึ่งชื่อเดิมคือบริการเทอร์มินัล:
- คุณต้องมี Microsoft ๓๖๕สำหรับแผนธุรกิจหรือแผน Office ๓๖๕ที่มีแอป Microsoft ๓๖๕สำหรับองค์กรเช่น Office ๓๖๕ Enterprise E3 หรือ Enterprise E5
   > [!NOTE] 
   > แอป Microsoft ๓๖๕สำหรับธุรกิจและแผนมาตรฐานของ Microsoft ๓๖๕ Business Premium ไม่รวมแอป Microsoft ๓๖๕สำหรับองค์กร
- คุณต้องเปิดใช้งานการ[เปิดใช้งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป microsoft ๓๖๕สำหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์ได้

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่[การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์:
- ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- ให้ดูที่[ตั้งค่าแอป Microsoft ๓๖๕สำหรับสถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)

ถ้าคุณต้องการติดตั้งแอป Microsoft ๓๖๕สำหรับ enterprise บน RDS จากศูนย์การจัดการ Microsoft ๓๖๕ ***ที่ใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:

1.    ตรวจสอบว่าคุณมีการสมัครใช้งานอะไรบ้าง [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)การ
2.    ถ้าจำเป็นให้สลับไปยังการสมัครใช้งานอื่น [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)การ
3.    ถ้า Office ได้รับการติดตั้งบนเซิร์ฟเวอร์ RDS แล้วโดยใช้การสมัครใช้งาน Microsoft อื่นๆให้ถอนการติดตั้ง ตัวอย่างเช่นโดยไปที่**แผงควบคุม**  >  **ถอนการติดตั้งโปรแกรม** ถอนการติดตั้งโดยใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) ถ้าคุณกำลังใช้งานปัญหา
4.    บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft ๓๖๕ด้วยบัญชีผู้ดูแลระบบของคุณและ[ติดตั้งแอป microsoft ๓๖๕สำหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)
5.    หลังจากติดตั้ง Office แล้ว ***อย่าเปิดหรือลงชื่อเข้า*** ใช้แอปพลิเคชัน office ใดๆ
6.    บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนต่อไปนี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอของคุณแล้วเลือก**เรียกใช้** ในกล่องเปิดให้พิมพ์**regedit**จากนั้นเลือก**ตกลง**
   2. เลือก **ใช่** เมื่อได้รับพร้อมท์ให้อนุญาตให้แก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ
   3. ใน Registry Editor ให้เพิ่มค่าสตริ **SharedComputerLicensing** ที่มีการตั้งค่า1ภายใต้ HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. บนเซิร์ฟเวอร์ RDS ให้***ลงชื่อเข้าใช้ในฐานะผู้ใช้***และ[ตรวจสอบว่าเปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์ไว้สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

