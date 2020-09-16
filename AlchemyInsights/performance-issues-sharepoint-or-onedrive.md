---
title: ปัญหาด้านประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771920"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน

SharePoint หรือ OneDrive อาจทำให้ไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานหรืออาจไม่พร้อมใช้งานหรืออาจแสดงข้อผิดพลาดของบริการที่ไม่พร้อมใช้งานหรือข้อผิดพลาด๕๐๓ด้วยเหตุผลหลายประการดังนี้
  
- ถ้าไซต์ SharePoint หรือ OneDrive ของคุณช้าหรือล่าช้าสำหรับผู้ใช้หลายคนอาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้ประสบปัญหาความล่าช้าหรือข้อผิดพลาดในการนำทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่
  
- ผู้ใช้อาจได้รับข้อผิดพลาดที่ *ไม่ว่างของ๕๐๓* เมื่อพยายามนำทางไปยังไซต์ SharePoint หรือ OneDrive ข้อผิดพลาดนี้อาจมีสาเหตุมาจากการควบคุมปริมาณภายในบริการ SharePoint SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint Online การควบคุมปริมาณจะจำกัดจำนวนการดำเนินการของผู้ใช้หรือการโทรที่พร้อมกัน (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้มีทรัพยากรมากเกินไป สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณให้ดูที่[หลีกเลี่ยงการปริมาณหรือการบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- ถ้าคุณพบประสิทธิภาพการทำงานที่ช้าลงด้วยไซต์หรือไซต์ SharePoint แบบ **คลาสสิก** หรือ **สมัยใหม่** ให้ใช้ [เครื่องมือการวินิจฉัยหน้า](https://aka.ms/perftool) เพื่อวิเคราะห์หน้า
  
- ถ้าคุณยังคงพบประสิทธิภาพการทำงานที่ช้าทั่วไปโปรดตรวจทานทรัพยากรที่ด้านล่างของบทความนี้: [บทนำสู่การปรับปรุงประสิทธิภาพการทำงานสำหรับ SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  