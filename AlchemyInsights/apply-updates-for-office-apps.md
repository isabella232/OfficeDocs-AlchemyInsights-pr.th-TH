---
title: ใช้การอัปเดตOfficeแอป
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969404"
---
# <a name="apply-updates-for-office-apps"></a>ใช้การอัปเดตOfficeแอป

ตามค่าเริ่มต้น การอัปเดตของแอป Office จะดาวน์โหลดฟรีโดยอัตโนมัติ และจะถูกใช้งานในเบื้องหลังโดยไม่มีการขัดจังหวะการใดๆ ของผู้ใช้ เมื่อต้องการเรียกใช้การอัปเดตด้วยตนเองถ้าคุณพบปัญหาในการใช้การอัปเดต ให้ดู[ติดตั้งOfficeต่างๆ](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) For more information, see [Troubleshoot installing Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

เมื่อต้องการจัดการOfficeต่างๆ ให้กับผู้ใช้ของคุณ ให้พิจารณาตัวเลือกเหล่านี้:

- เลือกตัวเลือกOfficeอัปเดตแชนเนลขององค์กรของคุณโดยยึดตามความถี่ของการอัปเดตที่ต้องการ เมื่อต้องการเรียนรู้วิธีการ ให้ดู ภาพรวมของ[แชนเนลการอัปเดตMicrosoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)อัปเดต

- ตัดสินใจว่าจะใช้การอัปเดตโดยอัตโนมัติจากอินเทอร์เน็ตหรือจากการแชร์ภายในองค์กร เมื่อต้องการเรียนรู้วิธี ให้ดู[เลือกวิธีการจัดการการอัปเดตMicrosoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)

- ตรวจทานOfficeการอัปเดต การตั้งค่าควบคุมวิธีการปรับใช้การอัปเดตกับเครื่องของผู้ใช้:

    - [กําหนดค่าการตั้งค่าการอัปเดตMicrosoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)
    - [กําหนดOfficeวิธีการอัปเดตหลังจากติดตั้ง](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

เมื่อปรับใช้Officeผู้ใช้หลายราย ให้ใช้เครื่องมือการกําหนดค่า Office เพื่อสร้างไฟล์การกําหนดค่าเพื่อการปรับใช้ และกําหนดค่าOfficeต่างๆ โดยใช้เครื่องมือการปรับใช้ Office For more info, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) and the Office Deployment [tool](https://go.microsoft.com/fwlink/p/?LinkID=626065).

- For an example of how to setup user groups to deploy Office s, see [Deploy Microsoft 365 Apps from a local source](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   พิจารณาใช้การตั้งค่า ForceAppShutdown Officeการอัปเดตของคุณจะไม่ถูกใช้กับผู้ใช้บางรายเนื่องจากแอปที่เปิดอยู่Officeบางแอป For more info, see the [FORCEAPPSHUTDOWN property (part of Property element)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element). 

**ดูเพิ่มเติม**

[ภาพรวมของกระบวนการอัปเดตMicrosoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)  
[ข้อมูลการเผยแพร่การอัปเดตMicrosoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)  
[จัดการการอัปเดตMicrosoft 365 Appsด้วย Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)  
