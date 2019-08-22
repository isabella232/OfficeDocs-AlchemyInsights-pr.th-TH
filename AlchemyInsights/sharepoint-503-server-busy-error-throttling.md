---
title: ควบคุมปริมาณออนไลน์ของ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559860"
---
# <a name="sharepoint-online-throttling"></a>ควบคุมปริมาณออนไลน์ของ SharePoint

ผู้ใช้อาจได้รับ 503 เซิร์ฟเวอร์ไม่ว่างผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ SharePoint หรือ OneDrive ได้ 

ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมภายในบริการ SharePoint ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร ถ้าได้รับควบคุมปริมาณคุณ 99% ของเวลาดังกล่าวจะ มีโค้ดแบบกำหนดเอง

สำหรับข้อมูลเพิ่มเติมในการควบคุมปริมาณให้ดู[Avoid การควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

ถ้าคุณเชื่อว่า ข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ คุณสามารถตรวจสอบถ้าไม่มีการบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)ที่ใช้งานอยู่

 ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า[ความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น

