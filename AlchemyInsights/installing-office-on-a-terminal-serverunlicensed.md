---
title: การติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์ - สิทธิ์
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498434"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้ง Office บนเทอร์มินัลเซิร์ฟเวอร์

สำหรับการจัดวาง ProPlus 365 Office บนเซิร์ฟเวอร์ของ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมคือชื่อบริการเทอร์มินัล:
  
- คุณต้องมีแผนการ Office 365 ที่มี Office 365 ProPlus เช่น E3 องค์กร 365 Office หรือองค์กร E5 แผน Office 365 ธุรกิจและค่าจ้างพิเศษธุรกิจ 365 Office ไม่มี Office 365 ProPlus

- คุณต้องเปิดใช้งาน[คอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

ถ้าคุณต้องการติดตั้ง Office 365 ProPlus ใน RDS จากพอร์ทัล Office 365***ซึ่งใช้การตั้งค่าติดตั้งเริ่มต้น***ให้ทำตามขั้นตอนเหล่านี้:
  
1. ตรวจสอบแผน Office 365 ใดที่คุณมี [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจำเป็น การสลับไปยัง Office 365 อื่นวางแผนไว้ [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office 365 อื่น ถอนการติดตั้ง ตัวอย่างเช่น ด้วยการไปที่'แผงควบคุม'\>ถอนการติดตั้งโปรแกรม ถอนใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังใช้งานเป็นการตัดสินค้าจากคลัง

4. บนเซิร์ฟเวอร์ RDS เข้าสู่ระบบของพอร์ทัล Office 365 กับบัญชีผู้ดูแลและ[ติดตั้ง Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากที่มีการติดตั้ง Office***ไม่เปิด หรือลงชื่อเข้าใช้ใน***โปรแกรมประยุกต์ Office ใด ๆ

6. บนเซิร์ฟเวอร์ RDS เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:

1. คลิกขวาปุ่มของหน้าต่างในมุมซ้ายมือด้านล่างของหน้าจอ และเลือกเรียกใช้ ในกล่องเปิด พิมพ์**regedit**และจากนั้น ให้เลือก'ตกลง'

2. เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้ใช้ตัวแก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ

3. ใน Registry Editor เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่าของ 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration

7. บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในชื่อผู้ใช้***และ[ตรวจสอบว่า เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งาน Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้น คำแนะนำการตั้งค่า และคำแนะนำในการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่[ปรับใช้ Office 365 ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)
  
เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  