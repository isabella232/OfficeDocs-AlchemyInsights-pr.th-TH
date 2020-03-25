---
title: เคล็ดลับนโยบาย DLP ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932605"
---
# <a name="dlp-policy-tip-issues"></a>ปัญหาคําแนะนํานโยบาย DLP

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**เคล็ดลับนโยบาย DLP**

เมื่อใช้**นโยบาย DLP**ผู้ใช้จะได้รับการแจ้งเตือนเกี่ยวกับการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย** ผู้ดูแลระบบสามารถกําหนดค่าคําแนะนํานโยบายให้แสดงขณะทดสอบนโยบาย DLP ของตน หรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้แบบเต็ม
  
เมื่อต้องการกําหนดค่านโยบายเคล็ดลับนโยบายนโยบาย DLP ของคุณในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบในโหมดการบังคับใช้แบบเต็ม ให้ทําดังนี้
  
- ตรวจสอบให้แน่ใจว่าได้**เปิดใช้งาน**เคล็ดลับนโยบายในกฎ DLP โดยใช้ขั้นตอน[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

- ตรวจสอบให้แน่ใจ**ว่าเนื้อหาของคุณตรงกับ****สิ่งที่จําเป็น**เพื่อทริกเกอร์กฎที่กล่าวถึงในบทความนี้[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- คําแนะนํานโยบายแสดงทั้งใน OWA และ Outlook อย่างไรก็ตาม เมื่อใช้**Outlook 2013 หรือรุ่นที่ใหม่กว่า** เงื่อนไขเหล่านี้จะแสดงอยู่ที่นี่:[เงื่อนไขที่ได้รับการสนับสนุนสําหรับ Outlook 2013 หรือรุ่นที่ใหม่กว่าสําหรับการแสดงคําแนะนํานโยบาย](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ให้ดูที่:[แสดงเคล็ดลับนโยบายสําหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  