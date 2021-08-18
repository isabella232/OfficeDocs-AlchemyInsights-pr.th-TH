---
title: การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล - ไม่มีใบอนุญาต
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322018"
---
# <a name="installing-office-on-a-terminal-server"></a>การติดตั้งOfficeเทอร์มินัลเซิร์ฟเวอร์

For deploying Microsoft 365 Apps for enterprise a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:
  
- คุณต้องมีการสมัครใช้งาน Microsoft 365ที่รวมMicrosoft 365 Apps for enterprise เช่น Office 365 Enterprise E3 หรือ Enterprise E5 แผนMicrosoft 365 Apps for business Microsoft 365 Apps for business Premiumและแผนบริการไม่รวมMicrosoft 365 Apps for enterprise

- คุณต้องเปิดใช้งาน [การเปิดใช้งานคอมพิวเตอร์ที่](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)แชร์

ถ้าคุณต้องการติดตั้งใน Microsoft 365 Apps for enterprise RDS จากศูนย์การจัดการ Microsoft 365 ***ซึ่งใช้การตั้งค่า*** การติดตั้งเริ่มต้น ให้ปฏิบัติตามขั้นตอนต่อไปนี้

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. ตรวจสอบMicrosoft 365การสมัครใช้งานที่คุณมี [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งานMicrosoft 365อื่น [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. ถ้าOfficeถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งานMicrosoft 365อื่นๆ ให้ถอนการติดตั้งออก ตัวอย่างเช่น โดยการไปที่ แผงควบคุม \> ถอนการติดตั้งโปรแกรม ถอนการติดตั้ง[โดยใช้ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)Microsoft ถ้าคุณพบปัญหา

4. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365ด้วยบัญชีผู้ดูแลระบบของคุณ[Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx)

5. หลังจากOfficeติดตั้ง ***แล้ว อย่าเปิดหรือลงชื่อเข้าใช้แอปพลิเคชัน*** ใดๆ Officeอื่น

6. บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยปฏิบัติตามขั้นตอนเหล่านี้:

1. คลิกขวาที่ปุ่มWindowsที่มุมซ้ายล่างของหน้าจอแล้วเลือก เรียกใช้ ในกล่อง เปิด ให้พิมพ์ **regedit** แล้วเลือก ตกลง

2. เลือก ใช่ เมื่อได้รับพร้อมท์ให้อนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ

3. ใน Registry Editor ให้เพิ่มค่าสตริง **ของ SharedComputerLicensing** ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration

7. บนเซิร์ฟเวอร์ RDS ให้ ***ลงชื่อเข้าใช้เป็นผู้ใช้ และตรวจสอบว่า*** เปิดใช้งานคอมพิวเตอร์ที่แชร์ [Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)หรือไม่

สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อแนะนําเบื้องต้น คําแนะนําการตั้งค่าและคําแนะนําเกี่ยวกับการติดตั้งแบบOfficeโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่ ปรับใช้โปรแกรมMicrosoft 365 Apps for enterprise[โดยใช้ Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  