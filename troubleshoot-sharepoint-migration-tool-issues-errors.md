---
title: การแก้ไขปัญหาเครื่องมือการโยกย้าย SharePoint และข้อผิดพลาด
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931137"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a>การแก้ไขปัญหาเครื่องมือการโยกย้าย SharePoint และข้อผิดพลาด

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**ปัญหาทั่วไปและข้อผิดพลาด**

คุณอาจพบปัญหาทั่วไปและข้อผิดพลาดบางอย่างเมื่อใช้เครื่องมือการโยกย้าย SharePoint (SPMT) โปรดอ้างอิงลิงก์ด้านล่างสําหรับข้อมูลเพิ่มเติม

* [การแก้ไขปัญหาและข้อผิดพลาดของ SPMT ทั่วไป](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [การแก้ไขปัญหาการติดตั้ง SPMT](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)