---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758749"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>สร้างกลุ่มไซต์ที่เชื่อมโยงใน SharePoint แบบออนไลน์

มีอยู่สองของปัญหาทั่วไปที่พบในขณะที่สร้าง หรือสร้างกลุ่มใหม่ให้เชื่อมต่อไซต์

 ถ้าคุณได้ลบกลุ่มและไซต์เชื่อมต่ออยู่ และต้องการที่สร้างไซต์อื่นที่ มี URL เดียวกัน คุณจำเป็นต้องการเอาไซต์ก่อนหน้า

ดาวน์โหลด[SPO จัดการ Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 สำหรับข้อมูลเพิ่มเติมในการเริ่มต้นใช้ powershell ดู[การเริ่มต้นใช้งานกับเชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

เอาไซต์ออกจากไซต์ถูกลบโดยใช้ cmdlet powershell[เอา SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

ถ้าคุณกำลังสร้างกลุ่มเชื่อมต่อไซต์ และได้รับคำเตือนกลุ่มอื่น ด้วยนามแฝงเหมือนกันอยู่แล้ว ตรวจสอบกลุ่มจาก[Office 365 จากศูนย์ดูแล](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)ที่มีอยู่หรือไม่ เมื่อต้องการแก้ไขปัญหา ไม่จำเป็นต้องลบกลุ่มที่มีอยู่ หรือสร้างไซต์ ด้วยนามแฝงแตกต่างกันกำหนด

มีวิธีต่าง ๆ ในการสร้าง และใช้กลุ่มสมัยใหม่กับ SharePoint

คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Office 365 สำหรับข้อมูลเพิ่มเติม ให้ดู[กลุ่ม Office 365 ineterface ผู้ใช้ SharePoint โดยใช้การเชื่อมต่อ](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)

เมื่อต้องการสร้างการเชื่อมโยงไซต์กลุ่ม Office 365 คุณจำเป็นต้องสร้างไซต์สำหรับทีม สำหรับข้อมูลเพิ่มเติม โปรดดู[สร้างไซต์สำหรับทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)

