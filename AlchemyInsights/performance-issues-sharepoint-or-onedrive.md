---
title: ปัญหาประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068439"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้า, ไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน

SharePoint หรือ OneDrive อาจทำงานช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานหรืออาจแสดงข้อผิดพลาดของบริการที่ไม่พร้อมใช้งานหรือ๕๐๓ด้วยเหตุผลหลายประการ:
  
- ถ้าไซต์ SharePoint หรือ OneDrive ของคุณช้าหรือล่าช้าสำหรับผู้ใช้หลายคนอาจมีปัญหาการบริการแบบถาวรที่ผู้ใช้พบความล่าช้าหรือข้อผิดพลาดการนำทางเป็นระยะๆเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ[แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่
  
- ผู้ใช้อาจได้รับ*๕๐๓เซิร์ฟเวอร์ไม่ว่าง*ข้อผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ SharePoint หรือ OneDrive ข้อผิดพลาดนี้อาจเกิดจากการควบคุมปริมาณภายในบริการ SharePoint SharePoint แบบออนไลน์ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์ การควบคุมปริมาณจะจำกัดจำนวนของการดำเนินการของผู้ใช้หรือการโทรที่เกิดขึ้นพร้อมกัน (โดยใช้สคริปต์หรือรหัส) เพื่อป้องกันไม่ให้ทรัพยากรมากเกินไป สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณการใช้งานโปรดหลีกเลี่ยงการใช้งาน[หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- ถ้าคุณพบกับประสิทธิภาพการทำงานที่ช้าด้วยไซต์หรือเพจ SharePoint แบบ**คลาสสิก**หรือ**สมัยใหม่**ให้ใช้[เครื่องมือวินิจฉัยหน้า](https://aka.ms/perftool)เพื่อวิเคราะห์เพจ
  
- หากคุณยังคงพบประสิทธิภาพการทำงานช้าทั่วไปโปรดตรวจทานทรัพยากรที่ด้านล่างของบทความนี้:[บทนำเกี่ยวกับการปรับประสิทธิภาพการทำงานสำหรับ SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=2024334)
  