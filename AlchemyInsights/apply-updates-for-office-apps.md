---
title: นำการอัปเดตสำหรับแอป Office ไปใช้
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
ms.openlocfilehash: 8306d1acafe48f8779a8c02db8e3fe2f5d5f0e95
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716768"
---
# <a name="apply-updates-for-office-apps"></a>นำการอัปเดตสำหรับแอป Office ไปใช้

ตามค่าเริ่มต้นการอัปเดตสำหรับ Office จะเป็นแบบฟรีดาวน์โหลดโดยอัตโนมัติและนำไปใช้ในพื้นหลังโดยไม่มีการขัดจังหวะของผู้ใช้ เมื่อต้องการเรียกใช้การอัปเดตด้วยตนเองถ้าคุณกำลังพบปัญหาในการใช้การอัปเดตให้ดู[ติดตั้งการอัปเดต Office](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) สำหรับข้อมูลเพิ่มเติมให้ดูที่[แก้ไขปัญหาการติดตั้ง Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)

เมื่อต้องการจัดการการอัปเดต Office สำหรับผู้ใช้ของคุณให้พิจารณาตัวเลือกเหล่านี้:

- เลือกช่องทางการอัปเดต Office ที่เหมาะสมสำหรับองค์กรของคุณโดยยึดตามความถี่ที่ต้องการของการอัปเดต เมื่อต้องการเรียนรู้วิธีการให้ดูที่[ภาพรวมของช่องทางการอัปเดตสำหรับแอป Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)

- ตัดสินใจว่าจะใช้การอัปเดตโดยอัตโนมัติจากอินเทอร์เน็ตหรือจากการใช้ร่วมกันภายในองค์กร เมื่อต้องการเรียนรู้วิธีการให้ดูที่[เลือกวิธีการจัดการการอัปเดตเป็น Microsoft ๓๖๕ Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)

- ตรวจทานการตั้งค่าการอัปเดต Office เพื่อควบคุมวิธีการนำการอัปเดตไปใช้กับเครื่องผู้ใช้ปลายทาง:

    - [กำหนดค่าการตั้งค่าการอัปเดตสำหรับแอป Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)
    - [กำหนดวิธีที่ Office ได้รับการอัปเดตหลังจากติดตั้ง](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)แล้ว

เมื่อปรับใช้แอป Office กับผู้ใช้หลายคนให้ใช้เครื่องมือกำหนดเองของ Office เพื่อสร้างไฟล์การกำหนดค่าสำหรับการปรับใช้และกำหนดค่าการอัปเดต Office โดยใช้เครื่องมือการปรับใช้ Office สำหรับข้อมูลเพิ่มเติมให้ดูที่[ภาพรวมของเครื่องมือกำหนดเองของ office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)และ[เครื่องมือการปรับใช้ office](https://go.microsoft.com/fwlink/p/?LinkID=626065)

- สำหรับตัวอย่างของวิธีการตั้งค่ากลุ่มผู้ใช้เพื่อปรับใช้การอัปเดต Office ให้ดูที่การ[ปรับใช้แอป Microsoft ๓๖๕จากแหล่งข้อมูลภายในเครื่อง](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)
-   พิจารณาใช้การตั้งค่า ForceAppShutdown ในกรณีที่การอัปเดต Office ไม่ได้ถูกนำไปใช้กับผู้ใช้บางรายเนื่องจากแอป Office ที่เปิดอยู่ สำหรับข้อมูลเพิ่มเติมให้ดูที่[คุณสมบัติ FORCEAPPSHUTDOWN (ส่วนหนึ่งขององค์ประกอบคุณสมบัติ)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element) 

**ดูเพิ่มเติม**

[ภาพรวมของกระบวนการอัปเดตสำหรับแอป Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)  
[วางจำหน่ายข้อมูลสำหรับการอัปเดตเป็นแอป Microsoft ๓๖๕](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)  
[จัดการการอัปเดตเป็นแอป microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า microsoft จุดสิ้น](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)สุด  
