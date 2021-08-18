---
title: การปรับใช้Microsoft 365 Apps for enterpriseการใช้งานที่แชร์บน RDS, Terminal Server หรือ VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325622"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้Microsoft 365 Apps for enterpriseการใช้งานที่แชร์บน RDS, Terminal Server หรือ VDI

เมื่อต้องการปรับใช้Microsoft 365 Apps for enterpriseโดยใช้ Remote Desktop Services (RDS) ซึ่งชื่อเดิมคือ Terminal Services ให้ทําดังนี้

- คุณต้องมีแผน Microsoft 365 For Business หรือแผน Office 365 ที่มีMicrosoft 365 Apps for enterprise เช่น Office 365 Enterprise E3 หรือ Enterprise E5
   **หมายเหตุ**: Microsoft 365 Apps for business Microsoft 365 Business Standardแผนบริการไม่รวมMicrosoft 365 Apps for enterprise
- คุณต้องเปิดใช้งาน [การเปิดใช้งานคอมพิวเตอร์ที่](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)แชร์

**หมายเหตุ**: คุณยังสามารถดาวน์โหลดและเรียกใช้ [Microsoft ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้งMicrosoft 365 Apps for enterpriseในโหมดเปิดใช้งานคอมพิวเตอร์ที่แชร์

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อเบื้องต้น คําแนะนําในการตั้งค่า และคําแนะนําเกี่ยวกับการติดตั้งแบบOffice โดยใช้เครื่องมือการปรับใช้ Microsoft 365 Apps for enterprise[ให้ดูที่](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)การปรับใช้บริการเดสก์ท็อประยะไกล

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ ให้ต่อไปนี้

- ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)ร่วมกัน
- ดู[ตั้งค่าMicrosoft 365 Apps for enterpriseสถานะการเปิดใช้งาน](https://go.microsoft.com/fwlink/?linkid=2109218)ใหม่

ถ้าคุณต้องการติดตั้งการติดตั้งMicrosoft 365 Apps for enterprise RDS จากศูนย์การจัดการ Microsoft 365 ***ซึ่งใช้การตั้งค่า*** การติดตั้งเริ่มต้น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ตรวจสอบการสมัครใช้งานที่คุณมี [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. ถ้าคุณOffice RDS โดยใช้การสมัครใช้งาน Microsoft อื่นๆ ให้ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่ **แผงควบคุม**  >  **ถอนการติดตั้ง** โปรแกรม ถอนการติดตั้ง[โดยใช้ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)Microsoft ถ้าคุณพบปัญหา
4. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365ด้วยบัญชีผู้ดูแลระบบของคุณ[Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx)
5. หลังจากOfficeติดตั้ง ***แล้ว อย่าเปิดหรือลงชื่อเข้าใช้*** แอปพลิเคชันใดๆ Officeอื่น
6. บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยปฏิบัติตามขั้นตอนเหล่านี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอ **แล้วเลือก** เรียกใช้ ในกล่อง เปิด ให้พิมพ์ **regedit****แล้วเลือก** ตกลง
   2. เลือก **ใช่** เมื่อได้รับพร้อมท์ให้อนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ
   3. ใน Registry Editor ให้เพิ่มค่าสตริง **ของ SharedComputerLicensing** ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration
   4. บนเซิร์ฟเวอร์ RDS ให้ ***ลงชื่อเข้าใช้เป็นผู้ใช้ และตรวจสอบว่า*** เปิดใช้งานคอมพิวเตอร์ที่แชร์ [Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)หรือไม่
