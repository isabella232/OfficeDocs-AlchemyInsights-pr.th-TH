---
title: การควบคุมปริมาณ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773866"
---
# <a name="sharepoint-online-throttling"></a>การควบคุมปริมาณ SharePoint Online

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**เซิร์ฟเวอร์๕๐๓มีข้อผิดพลาดที่ไม่ว่าง**

ผู้ใช้อาจได้รับข้อผิดพลาดที่ไม่ว่างของ๕๐๓เมื่อพยายามนำทางไปยังไซต์ SharePoint หรือ OneDrive 

ข้อผิดพลาดนี้อาจมีสาเหตุมาจากการควบคุมปริมาณภายในบริการ SharePoint SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint Online การควบคุมปริมาณจะจำกัดจำนวนการดำเนินการของผู้ใช้หรือการโทรที่พร้อมกัน (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้มีทรัพยากรมากเกินไป 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณให้ดูที่[หลีกเลี่ยงการปริมาณหรือการบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณคุณสามารถตรวจสอบว่ามีการบำรุงรักษาที่ใช้งานอยู่ในผู้เช่าของคุณหรือไม่โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)

 สุดท้ายให้ตรวจสอบให้แน่ใจว่าคุณได้เยี่ยมชมหน้า [สถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth) เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้น

