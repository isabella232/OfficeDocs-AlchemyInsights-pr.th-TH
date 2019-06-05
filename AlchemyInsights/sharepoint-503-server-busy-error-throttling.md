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
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716945"
---
# <a name="sharepoint-online-throttling"></a>ควบคุมปริมาณออนไลน์ของ SharePoint

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ผู้ใช้อาจได้รับ 503 เซิร์ฟเวอร์ไม่ว่างผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ Sharepoint หรือ OneDrive ได้</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมภายในบริการ Sharepoint ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร ถ้าได้รับควบคุมปริมาณคุณ 99% ของเวลาดังกล่าวจะ มีโค้ดแบบกำหนดเอง</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำหรับข้อมูลเพิ่มเติมในการควบคุมปริมาณให้ดู<a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid การควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ถ้าคุณเชื่อว่า ข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ คุณสามารถตรวจสอบถ้าไม่มีการบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง<a href="https://portal.office.com/adminportal/home#/MessageCenter">ศูนย์ข้อความ</a>ที่ใช้งานอยู่ ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า<a href="https://portal.office.com/adminportal/home#/servicehealth">ความสมบูรณ์ของบริการ</a>เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span></p> <p>&nbsp;</p>


