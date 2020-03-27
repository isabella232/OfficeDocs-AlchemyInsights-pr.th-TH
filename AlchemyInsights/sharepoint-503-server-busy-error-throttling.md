---
title: การควบคุมปริมาณแบบออนไลน์ของ SharePoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958754"
---
# <a name="sharepoint-online-throttling"></a>การควบคุมปริมาณแบบออนไลน์ของ SharePoint

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ข้อผิดพลาดของเซิร์ฟเวอร์ 503 ไม่ว่าง**

ผู้ใช้อาจได้รับเซิร์ฟเวอร์ 503 ไม่ว่างข้อผิดพลาดเมื่อพยายามที่จะนําทางไปยังไซต์ SharePoint หรือ OneDrive 

ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมปริมาณภายในบริการ SharePoint SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์ การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป 

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณ ให้ดูที่[หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ[Message center](https://portal.office.com/adminportal/home#/MessageCenter)

 ตรวจสอบคําแนะนํา/เหตุการณ์ที่อาจเกิดขึ้น[Service Health](https://portal.office.com/adminportal/home#/servicehealth)

