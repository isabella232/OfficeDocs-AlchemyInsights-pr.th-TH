---
title: Web Part Yammer ใน SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198384"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Web Part Yammer ใน SharePoint

การสนทนา Yammer และ Yammer เน้น Web Part ช่วยเพิ่มการทํางานร่วมกันบนเพจ SharePoint สมัยใหม่และแบบคลาสสิก สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การสนทนา Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)และ[ไฮไลต์ของ Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)    

Web Part การสนทนา Yammer สมัยใหม่กําลังถูกปรับปรุงให้ประสบการณ์ใช้งาน Yammer ใหม่ และพร้อมใช้งานสําหรับผู้เช่าที่นําออกใช้เป้าหมาย เปิดตัว GA ได้เริ่มต้นแล้ว คุณลักษณะใหม่รวมถึงความสามารถในการเริ่มต้นการสนทนากับโพสต์ใด ๆ (คําถาม, โพลล์, สรรเสริญ) และทําเครื่องหมายคําตอบที่ดีที่สุดโดยตรงจาก SharePoint สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ข้อกําหนดของลูกค้าและคําถามที่ถามบ่อยเกี่ยวกับ Yammer ใหม่](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)

 เมื่อต้องการทําความเข้าใจว่า Web Part และการกําหนดค่าใดเหมาะกับคุณ ให้ดูที่[ใช้ Web Part Yammer ใน SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)  

**การใช้ Web Part กับเซิร์ฟเวอร์ SharePoint**  

Web Part สามารถใช้ในเพจสมัยใหม่และคลาสสิกภายในสภาพแวดล้อมในสถานที่

- สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเพจสมัยใหม่ ให้ดูที่[การเพิ่มตัวดึงข้อมูล Yammer ไปยังเพจสมัยใหม่ใน SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019) 
- สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเพจแบบคลาสสิก ให้ดูที่[การเพิ่มตัวดึงข้อมูล Yammer ไปยังเพจแบบคลาสสิคใน SharePoint Servers 2013, 2016 และ 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)

**ฝัง Yammer**  

ใช้เครื่องมือการกําหนดค่าฝังเพื่อทดสอบการใช้งานฝัง การปรับปรุงในอนาคตเพื่อฝังจะเปิดใช้งานประสบการณ์การใช้งาน Yammer ใหม่ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[เครื่องมือการกําหนดค่าการฝัง Yammer](https://aka.ms/YammerEmbedConfigureTool) เมื่อต้องการทําความเข้าใจคอมโพเนนต์ Yammer Embed ให้ดียิ่งขึ้น ให้ดูที่[ฝังตัวดึงข้อมูล](https://aka.ms/YammerDevDocs)

**ปัญหาที่ทราบและข้อจํากัด**

- ID กลุ่มไม่พร้อมใช้งานจาก Url Yammer ใหม่ ซึ่งมีการเปลี่ยนแปลง สลับกลับไปยังโหมดคลาสสิกเพื่อรับข้อมูลกลุ่มหรือไอดีอื่นจาก URL
- ไม่สนับสนุนโดเมนแบบกําหนดเอง (vanity)
- Yammer ฝังไม่ได้รับการปรับให้เหมาะสมสําหรับอุปกรณ์เคลื่อนที่ ใช้เพจสมัยใหม่กับ Web Part การสนทนา Yammer เพื่อประสบการณ์ที่ดีที่สุด
- ชุดรูปแบบแบบกําหนดเองอาจมีผลต่อลักษณะที่ปรากฏและการใช้งานของ Web Part การสนทนา Yammer เปิดกรณีสนับสนุนเพื่อรายงานปัญหา