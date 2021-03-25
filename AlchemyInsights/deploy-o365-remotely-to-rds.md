---
title: การปรับใช้แอป Microsoft 365 ขององค์กรเพื่อใช้ที่แชร์บน RDS, Terminal Server หรือ VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200692"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>การปรับใช้แอป Microsoft 365 ขององค์กรเพื่อใช้ที่แชร์บน RDS, Terminal Server หรือ VDI

เมื่อต้องการปรับใช้แอป Microsoft 365 For enterprise โดยใช้ Remote Desktop Services (RDS) ชื่อเดิมคือ Terminal Services ให้ทําดังนี้

- คุณต้องมีแผน Microsoft 365 For Business หรือแผน Office 365 ที่มีแอป Microsoft 365 For Enterprise เช่น Office 365 Enterprise E3 หรือ Enterprise E5
   > [!NOTE]
   > Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.
- คุณต้องเปิดใช้งาน [การเปิดใช้งานคอมพิวเตอร์ที่](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)แชร์

> [!NOTE]
> คุณยังสามารถดาวน์โหลดและเรียกใช้ตัวช่วยการสนับสนุน [และการกู้คืนของ Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป Microsoft 365 for Enterprise ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อแนะนําเบื้องต้น คําแนะนําการตั้งค่า และคําแนะนําเกี่ยวกับการติดตั้งแบบปรับแต่งเองโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่ การปรับใช้แอป [Microsoft 365 สําหรับองค์กรโดยใช้บริการ](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)เดสก์ท็อประยะไกล

เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์:

- ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์กับแอป Microsoft 365 for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- ดู[รีเซ็ตแอป Microsoft 365 สถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)

ถ้าคุณต้องการติดตั้งแอป Microsoft 365 for enterprise บน RDS จากศูนย์การจัดการ Microsoft 365 ซึ่ง ***ใช้*** การตั้งค่าการติดตั้งเริ่มต้น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ตรวจสอบการสมัครใช้งานที่คุณมี [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น [เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft อื่นๆ ให้ถอนการติดตั้ง ตัวอย่างเช่น โดยไปที่ **แผงควบคุม**  >  **ถอนการติดตั้งโปรแกรม** ถอนการติดตั้ง [โดยใช้ตัวช่วยการสนับสนุนและ](https://aka.ms/SARA-OfficeUninstall-Alchemy) การกู้คืนของ Microsoft ถ้าคุณพบปัญหา
4. บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้งแอป Microsoft 365 for Enterprise](https://portal.office.com/OLS/MySoftware.aspx)
5. หลังจากติดตั้ง Office ***แล้ว อย่าเปิดหรือลงชื่อเข้าใช้*** แอปพลิเคชัน Office ใดๆ
6. บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยปฏิบัติตามขั้นตอนเหล่านี้:
   1. คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอและเลือก **เรียกใช้** ในกล่อง เปิด ให้พิมพ์ **regedit****แล้วเลือก** ตกลง
   2. เลือก **ใช่** เมื่อได้รับพร้อมท์ให้อนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ
   3. ใน Registry Editor ให้เพิ่มค่าสตริง **ของ SharedComputerLicensing** ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration
   4. บนเซิร์ฟเวอร์ RDS ให้ ***ลงชื่อเข้าใช้เป็นผู้ใช้ และตรวจสอบว่าเปิดใช้งาน*** การเปิดใช้งานคอมพิวเตอร์ที่แชร์แล้ว [ในแอป Microsoft 365 For Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
