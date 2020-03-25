---
title: การโยกย้าย SharePoint กับ SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931569"
---
# <a name="sharepoint-migration-with-spmt"></a>การโยกย้าย SharePoint กับ SPMT

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**เครื่องมือการโยกย้าย SharePoint**

ออกแบบมาเพื่อใช้สําหรับการย้ายตั้งแต่ชุดเล็กที่สุดของไฟล์เพื่อการย้ายองค์กรขนาดใหญ่เครื่องมือการโยกย้าย SharePoint จะช่วยให้คุณสามารถถ่ายโอนข้อมูลของคุณไปยังเมฆและใช้ประโยชน์จากการทํางานร่วมกันใหม่ล่าสุด, ปัญญา, และ โซลูชันการรักษาความปลอดภัยด้วย Office 365

- [ดาวน์โหลด และติดตั้งเครื่องมือการโยกย้าย SharePoint](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [การแก้ไขปัญหาและข้อผิดพลาดของ SPMT ทั่วไป](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [การแก้ไขปัญหาการติดตั้ง SPMT](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
