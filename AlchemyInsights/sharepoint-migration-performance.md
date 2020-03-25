---
title: ประสิทธิภาพการโยกย้าย SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932407"
---
# <a name="sharepoint-migration-performance"></a>ประสิทธิภาพการโยกย้าย SharePoint

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**ประสิทธิภาพการโยกย้าย**

ประสิทธิภาพการโยกย้ายอาจได้รับผลกระทบจากโครงสร้างพื้นฐานของเครือข่าย ขนาดไฟล์ เวลาการย้าย และการควบคุมปริมาณ การทําความเข้าใจสิ่งเหล่านี้จะช่วยให้คุณวางแผนและเพิ่มประสิทธิภาพในการย้ายข้อมูล

สําหรับข้อมูลเพิ่มเติมโปรดไปที่ลิงค์ด้านล่าง

- [ความเร็วการโยกย้ายของ Sharepoint แบบออนไลน์และ ODB](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [ดาวน์โหลด และติดตั้งเครื่องมือการโยกย้าย SharePoint](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
