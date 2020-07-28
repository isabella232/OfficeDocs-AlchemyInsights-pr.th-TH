---
title: นําการปรับปรุงสําหรับแอป Office ไปใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: b5952feaac7ac51faed2a3399c68a87a4227b165
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440152"
---
# <a name="apply-updates-for-office-apps"></a>นําการปรับปรุงสําหรับแอป Office ไปใช้

โดยค่าเริ่มต้น การปรับปรุงสําหรับ Office Apps จะฟรี ดาวน์โหลดโดยอัตโนมัติ และนําไปใช้ในพื้นหลังโดยผู้ใช้ใด ๆ เมื่อต้องการเรียกใช้การปรับปรุงด้วยตนเองถ้าคุณกําลังเรียกใช้เป็นปัญหาในการใช้การปรับปรุง ให้ดูที่[ติดตั้งโปรแกรมปรับปรุงของ Office](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การแก้ไขปัญหาการติดตั้ง Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)

เมื่อต้องการจัดการการปรับปรุง Office สําหรับผู้ใช้ของคุณ ให้พิจารณาตัวเลือกเหล่านี้

- เลือกช่องทางการปรับปรุง Office ที่เหมาะสมสําหรับองค์กรของคุณตามความถี่ของการอัปเดตที่ต้องการ เมื่อต้องการเรียนรู้วิธีการ ให้ดูที่[ภาพรวมของช่องทางการปรับปรุงสําหรับ Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)

- ตัดสินใจว่าจะใช้การปรับปรุงโดยอัตโนมัติจากอินเทอร์เน็ตหรือจากหุ้นในสถานที่ เมื่อต้องการเรียนรู้วิธีการ ให้ดูที่[การเลือกวิธีจัดการการปรับปรุงสําหรับแอป Microsoft 365](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)

- ตรวจทานการตั้งค่าการปรับปรุง Office เพื่อควบคุมวิธีการใช้โปรแกรมปรับปรุงกับเครื่องจักรของผู้ใช้:

    - [กําหนดค่าการตั้งค่าการปรับปรุงสําหรับแอป Microsoft 365](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)
    - [กําหนดวิธี Office ได้รับการปรับปรุงหลังจากที่มีการติดตั้ง](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

เมื่อปรับใช้โปรแกรมประยุกต์ Office ให้กับผู้ใช้หลายคน ให้ใช้เครื่องมือกําหนดเองของ Office เพื่อสร้างแฟ้มการกําหนดค่าสําหรับการปรับใช้ และกําหนดค่าโปรแกรมปรับปรุง Office โดยใช้เครื่องมือการปรับใช้ Office สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ภาพรวมของเครื่องมือการกําหนดเองของ Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)และ[เครื่องมือการปรับใช้ Office](https://go.microsoft.com/fwlink/p/?LinkID=626065)

- สําหรับตัวอย่างวิธีการตั้งค่ากลุ่มผู้ใช้เพื่อปรับใช้การปรับปรุง Office ให้ดูที่[การปรับใช้แอป Microsoft 365 จากแหล่งที่อยู่ภายในเครื่อง](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)
-   พิจารณาใช้การตั้งค่า ForceAppShutdown ในกรณีที่โปรแกรมปรับปรุง Office จะไม่ได้รับการปรับใช้กับผู้ใช้สองสามคนเนื่องจากเปิดแอป Office สําหรับข้อมูลเพิ่มเติม ให้ดู[FORCEAPPSHUTDOWN คุณสมบัติ (ส่วนหนึ่งขององค์ประกอบคุณสมบัติ)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element) 

**ดู**

[ภาพรวมของกระบวนการปรับปรุงสําหรับแอป Microsoft 365](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)  
[ข้อมูลการนําออกใช้สําหรับการปรับปรุงไปยัง Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)  
[จัดการการปรับปรุงโปรแกรมประยุกต์ Microsoft 365 ด้วยตัวจัดการการตั้งค่าคอนฟิกปลายทางของ Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)  
