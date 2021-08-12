---
title: ปัญหาเกี่ยวกับประสิทธิภาพการSharePointหรือOneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911861"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointหรือOneDriveช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานได้โดยผู้ใช้หลายราย

SharePointหรือOneDriveอาจช้า เข้าถึงไม่ได้ หรือไม่พร้อมใช้งาน หรืออาจแสดงบริการไม่พร้อมใช้งาน หรือข้อผิดพลาด 503 เนื่องจากสาเหตุหลายประการ ดังนี้
  
- ถ้าไซต์ SharePoint หรือ OneDrive ของคุณช้าหรือล่าช้าไปโดยผู้ใช้หลายราย อาจมีปัญหาบริการชั่วคราวที่ผู้ใช้พบความล่าช้าหรือข้อผิดพลาดในการนําทางเป็นระยะเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ [แดชบอร์ดสถานภาพ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) บริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่
  
- ผู้ใช้อาจได้รับข้อผิดพลาด *503 เซิร์ฟเวอร์ไม่ว่าง* เมื่อพยายามนําทางSharePointหรือOneDriveอื่น ข้อผิดพลาดนี้อาจเกิดจากการควบคุมปริมาณภายในSharePointบริการของคุณ SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือที่ดีที่สุดของSharePointบริการออนไลน์ของคุณ การควบคุมจํานวนจะจํากัดจํานวนการกระทาของผู้ใช้หรือการโทรพร้อมกัน (ตามสคริปต์หรือโค้ด) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- ถ้าคุณพบประสิทธิภาพการช้าลงด้วย **ไซต์****หรือSharePoint** แบบคลาสสิกหรือทันสมัย ให้ใช้เครื่องมือ [การวินิจฉัย](https://aka.ms/perftool)หน้าเพื่อวิเคราะห์หน้า
  
- ถ้าคุณยังคงพบประสิทธิภาพการช้าทั่วไป โปรดตรวจสอบแหล่งข้อมูลที่ด้านล่างของบทความนี้: บทนําสู่การปรับปรุงประสิทธิภาพ[การ](https://go.microsoft.com/fwlink/?linkid=2024334)SharePoint Online
  