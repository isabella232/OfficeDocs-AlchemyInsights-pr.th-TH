---
title: การเพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051120"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>ปัญหาเมื่อสร้างหรือจัดกลุ่มไซต์ที่เชื่อมต่อใน SharePoint แบบออนไลน์

มีปัญหาที่พบบ่อยสองประการที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกับกลุ่มใหม่

 หากคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นด้วย URL เดียวกันคุณจะต้องเอาไซต์ก่อนหน้าออกอย่างถาวร

ดาวน์โหลด[เชลล์จัดการการบริหาร](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน powershell โปรดดูที่[การเริ่มต้นใช้งานเชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ cmdlet powershell ของการ[เอาออก SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

หากคุณกำลังสร้างไซต์ที่เชื่อมต่อกับกลุ่มและได้รับคำเตือนกลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้วให้ตรวจสอบกลุ่มที่มีอยู่จาก[Office ๓๖๕จากศูนย์การจัดการ](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups) เมื่อต้องการแก้ไขปัญหานี้ให้ลบกลุ่มที่มีอยู่ถ้าไม่ต้องการอีกต่อไปหรือสร้างไซต์ด้วยนามแฝงอื่นที่กำหนดไว้

มีหลายวิธีในการสร้างและใช้กลุ่มที่ทันสมัยกับ SharePoint

คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับกลุ่ม Office ๓๖๕ได้ สำหรับข้อมูลเพิ่มเติมโปรดดูที่[การเชื่อมต่อกลุ่ม Office ๓๖๕โดยใช้ ineterface ผู้ใช้ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)

หากต้องการสร้างไซต์ที่เชื่อมต่อกับกลุ่ม Office ๓๖๕คุณจะต้องสร้างไซต์ทีม สำหรับข้อมูลเพิ่มเติมให้ดู[สร้างไซต์ทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)

