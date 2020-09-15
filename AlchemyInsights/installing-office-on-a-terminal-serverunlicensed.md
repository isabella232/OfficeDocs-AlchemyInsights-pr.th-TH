---
title: การติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์-สิทธิ์การใช้งาน
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663136"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล

สำหรับการปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรบน Windows Server โดยใช้บริการเดสก์ท็อประยะไกล (RDS) ซึ่งชื่อเดิมคือบริการเทอร์มินัล:
  
- คุณต้องมีการสมัครใช้งาน Microsoft ๓๖๕ที่มีแอป Microsoft ๓๖๕สำหรับองค์กรเช่น Office ๓๖๕ Enterprise E3 หรือ Enterprise E5 แอป Microsoft ๓๖๕สำหรับธุรกิจและแอป Microsoft ๓๖๕สำหรับแผน business Premium ไม่รวมแอป Microsoft ๓๖๕สำหรับองค์กร

- คุณจำเป็นต้องเปิดใช้งานการเปิดใช้[งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

ถ้าคุณต้องการติดตั้งแอป Microsoft ๓๖๕สำหรับ enterprise บน RDS จากศูนย์การจัดการ Microsoft ๓๖๕ ***ที่ใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้

> [!TIP]
> นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป microsoft ๓๖๕สำหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์ได้
  
1. ตรวจสอบว่าคุณมีการสมัครใช้งาน Microsoft ๓๖๕อะไรบ้าง [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจำเป็นให้สลับไปยังการสมัครใช้งาน Microsoft ๓๖๕อื่น [เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. ถ้า Office ได้รับการติดตั้งบนเซิร์ฟเวอร์ RDS แล้วโดยใช้การสมัครใช้งาน Microsoft ๓๖๕อื่นๆให้ถอนการติดตั้ง ตัวอย่างเช่นโดยไปที่แผงควบคุม \> ถอนการติดตั้งโปรแกรม ถอนการติดตั้งโดยใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) ถ้าคุณกำลังใช้งานปัญหา

4. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft ๓๖๕ด้วยบัญชีผู้ดูแลระบบของคุณและ[ติดตั้งแอป microsoft ๓๖๕สำหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากติดตั้ง Office แล้ว ***อย่าเปิดหรือลงชื่อเข้า*** ใช้แอปพลิเคชัน office ใดๆ

6. บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนต่อไปนี้:

1. คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอของคุณแล้วเลือกเรียกใช้ ในกล่องเปิดให้พิมพ์ **regedit**จากนั้นเลือกตกลง

2. เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้แก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ

3. ใน Registry Editor ให้เพิ่มค่าสตริ **SharedComputerLicensing** ที่มีการตั้งค่า1ภายใต้ HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. บนเซิร์ฟเวอร์ RDS ให้***ลงชื่อเข้าใช้ในฐานะผู้ใช้***และ[ตรวจสอบว่าเปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์ไว้สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นการตั้งค่าคำแนะนำและคำแนะนำในการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่[การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  