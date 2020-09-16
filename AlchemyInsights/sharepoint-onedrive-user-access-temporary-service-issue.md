---
title: ปัญหาด้านประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771263"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน

ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)

**เพิ่มและสิทธิ์การใช้งานผู้ใช้**

ตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**กำหนดสิทธิ์**

ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึงโปรดตรวจสอบให้แน่ใจว่ามีการกำหนด[ระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**พิจารณาการใช้ฟีเจอร์การร้องขอการเข้าถึง**

[ฟีเจอร์การร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)ช่วยให้ผู้อื่นสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับสิทธิ์ในการดู

**อนุญาตสคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาในการเข้าถึงถูกปฏิเสธ**

มีบางสถานการณ์ที่การอนุญาตให้ใช้ฟีเจอร์ *สคริปต์แบบกำหนดเอง* อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ สำหรับรายการของฟีเจอร์ที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานฟีเจอร์นี้ โปรดเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

