---
title: ปัญหาประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750575"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้า, ไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน

ถ้าเว็บไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร [ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)

**เพิ่มและอนุญาตให้ผู้ใช้**

ตรวจสอบให้แน่ใจว่าคุณได้[มอบหมายใบอนุญาตให้กับผู้ใช้ใน Office ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)


**กำหนดสิทธิ์**

ถ้าผู้ใช้ได้รับการกำหนดใบอนุญาต Sharepoint และยังคงได้รับข้อความการเข้าถึงถูกปฏิเสธโปรดตรวจสอบให้แน่ใจว่ามีการกำหนด[ระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**

[คุณลักษณะการร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)ช่วยให้ผู้คนสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขาไม่ได้รับอนุญาตให้ดูได้ในขณะนี้

**อนุญาตสคริปต์ที่กำหนดเองอาจทำให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**

มีบางสถานการณ์ที่การอนุญาตให้ใช้คุณลักษณะของ*สคริปต์ที่กำหนดเอง*อาจนำเสนอการเข้าถึงถูกปฏิเสธ สำหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะนี้ โปรดเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

