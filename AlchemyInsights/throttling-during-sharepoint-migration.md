---
title: การควบคุมปริมาณในระหว่างการโยกย้าย SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958917"
---
# <a name="sharepoint-throttling"></a>การควบคุมปริมาณ SharePoint

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**การควบคุมปริมาณแบบออนไลน์ของ SharePoint**

SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์ การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป

สําหรับข้อมูลเพิ่มเติมกรุณาเยี่ยมชมลิงค์ด้านล่าง:

- [หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [การย้ายข้อมูลและการควบคุมปริมาณ SPO](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [ออนไลน์และ OneDrive ความเร็วในการโยกย้าย](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [จัดการการควบคุมปริมาณ SharePoint แบบออนไลน์ โดยใช้กลับชี้แจงออก](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [การวางแผนกําลังการผลิตและการทดสอบโหลด SharePoint ออนไลน์](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [ฉันประสบประสิทธิภาพการทํางานที่ไม่ดีหรือการควบคุมปริมาณในระหว่างการย้าย](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)