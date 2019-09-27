---
title: การติดตั้งสำนักงานบนเซิร์ฟเวอร์เทอร์มินัล-ใบอนุญาต
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205428"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล

สำหรับการจัดวาง Office ๓๖๕ ProPlus บนเซิร์ฟเวอร์ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:
  
- คุณต้องมีแผน Office ๓๖๕ที่ประกอบด้วย Office ๓๖๕ ProPlus เช่น Office ๓๖๕เอ็นเตอร์ไพรส์ E3 หรือองค์กร E5 แผนพรีเมียม Office ๓๖๕ธุรกิจและ Office ๓๖๕ไม่รวม Office ๓๖๕ ProPlus

- คุณต้องเปิดการใช้[งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

ถ้าคุณต้องการติดตั้ง Office ๓๖๕ ProPlus บน RDS จากศูนย์ดูแล Microsoft ๓๖๕***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้

> [!TIP]
> นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Office ๓๖๕ ProPlus ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน
  
1. ตรวจสอบว่าคุณมีแผน Office ๓๖๕ใดบ้าง [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจำเป็นให้สลับไปยังแผน Office ๓๖๕อื่น [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office ๓๖๕อื่นๆที่มีอยู่ให้ถอนการติดตั้ง ตัวอย่างเช่นโดยไปที่ ' แผง\>ควบคุม ' ถอนการติดตั้งโปรแกรม ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังทำงานเป็นปัญหา

4. บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์ดูแลของ Microsoft ๓๖๕กับบัญชีผู้ดูแลระบบของคุณและ[ติดตั้ง Office ๓๖๕ ProPlus](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากติดตั้ง Office แล้ว***อย่าเปิดหรือลงชื่อเข้า***ใช้โปรแกรมประยุกต์ office ใดๆ

6. บนเซิร์ฟเวอร์ RDS เปิดการใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:

1. คลิกขวาที่ปุ่ม Windows ในมุมด้านซ้ายมือล่างของหน้าจอของคุณและเลือกเรียกใช้ ในกล่องเปิดพิมพ์**regedit**และจากนั้นให้เลือก ' ตกลง '

2. เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทำการเปลี่ยนแปลงอุปกรณ์ของคุณ

3. ในตัวแก้ไขรีจิสทรีเพิ่มค่าสตริงของการอนุญาตให้ใช้**สิทธิ์ Sharedคอมพิวเตอร์**ที่มีการตั้งค่าของ1ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้ปลาย***ทางและตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้[ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำในการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่การจัดวาง[office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)
  
หากต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโปรดดูที่การ[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  