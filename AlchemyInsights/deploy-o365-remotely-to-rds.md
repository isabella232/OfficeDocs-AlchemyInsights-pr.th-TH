---
title: การปรับใช้Microsoft 365 Appsการใช้งานที่แชร์บน RDS, Terminal Server หรือ VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077269"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้Microsoft 365 Appsการใช้งานที่แชร์บน RDS, Terminal Server หรือ VDI

เมื่อต้องการปรับใช้Microsoft 365 Appsโดยใช้ Remote Desktop Services (RDS) ซึ่งชื่อเดิมคือ Terminal Services คุณต้องทําสิ่งต่อไปนี้

- ใช้การแก้ไขง่ายๆ เพื่อเปิดใช้งาน TLS 1.2 เป็นค่าเริ่มต้น ถ้าคุณใช้งาน Windows เวอร์ชันที่เก่ากว่า (เช่น Windows 7 SP1, Windows Server 2008 R2) For easy fix and more information, [see Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- มีแผนที่รวมMicrosoft 365 Apps for enterprise (Office 365บวก) ตัวอย่างเช่น Office 365 E3 หรือ Microsoft 365 E5 หรือแผนใดๆ ที่มี Project หรือ Visio เวอร์ชันเดสก์ท็อป เช่น Project Plan 3 หรือ Visio Plan 2 หรือแผน Microsoft 365 Business Premium ซึ่งรวมถึงแผน Microsoft 365 Apps for business ด้วย
- เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์ For more information, see [Overview of shared computer activation for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**หมายเหตุ**: เมื่อต้องการMicrosoft 365 Appsในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์ ให้ดาวน์โหลดและเรียกใช้ Microsoft [ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal) สําหรับรายละเอียดเกี่ยวกับข้อเบื้องต้น คําแนะนําในการตั้งค่า และคําแนะนําเพื่อปรับแต่งการติดตั้งโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่ ปรับใช้Microsoft 365 Apps[โดยใช้ Remote Desktop Services](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ ให้ดูที่

- [แก้ไขปัญหาการเปิดใช้งานคอมพิวเตอร์ที่แชร์Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [ตั้งค่าสถานะMicrosoft 365 Apps for enterpriseเปิดใช้งานใหม่](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

ถ้าคุณต้องการติดตั้ง RDS Microsoft 365 Apps RDS จากศูนย์การจัดการ Microsoft 365 ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ตรวจสอบว่าMicrosoft 365ของคุณมีแผนใด หากต้องการข้อมูลเพิ่มเติม โปรดดู [ฉันมีการสมัครใช้งานแบบ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)ใด

1. ถ้าจําเป็น ให้สลับไปยังMicrosoft 365อื่น หากต้องการข้อมูลเพิ่มเติม โปรดดู [อัปเกรดเป็นแผน](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)อื่น

1. ถ้าMicrosoft 365 Appsถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผนอื่นที่เข้ากันไม่ได้ ให้ถอนการติดตั้งโดยไปที่  >  **แผงควบคุม ถอนการติดตั้ง** โปรแกรม ถ้าคุณพบปัญหา ให้ถอนการติดตั้งโดยดาวน์โหลด Microsoft[ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365บัญชีผู้ดูแลระบบของคุณ[และติดตั้งOffice](https://portal.office.com/OLS/MySoftware.aspx)

   หลังจากOfficeติดตั้งแล้ว อย่าเปิดหรือลงชื่อเข้าใช้แอปพลิเคชันใดๆ Officeอื่น

1. บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรี:

   1. คลิกขวาที่ปุ่มWindowsที่มุมซ้ายล่างของหน้าจอแล้วเลือก **เรียกใช้** ในกล่อง เปิด ให้พิมพ์ **regedit****แล้วเลือก** ตกลง

   1. เมื่อได้รับพร้อมท์ให้อนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ **ให้เลือก** ใช่

   1. ใน Registry Editor ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration ให้เพิ่มค่าสตริง **ของ SharedComputerLicensing** ด้วย **การตั้งค่า 1**

1. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ในฐานะผู้ใช้ และตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่แชร์Microsoft 365 Appsหรือไม่ 

   For details, see [Verify that shared computer activation is enabled for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).