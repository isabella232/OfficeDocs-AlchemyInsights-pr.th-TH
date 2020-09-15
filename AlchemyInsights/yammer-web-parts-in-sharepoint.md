---
title: Web part ของ Yammer ใน SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664369"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Web part ของ Yammer ใน SharePoint

การสนทนา yammer และ Yammer ไฮไลต์ web part เพิ่มประสิทธิภาพการทำงานร่วมกันบนหน้า SharePoint ที่ทันสมัยและคลาสสิก สำหรับข้อมูลเพิ่มเติมให้ดูที่[การสนทนา yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)และ[ไฮไลต์ของ yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)    

Web part การสนทนา Yammer ที่ทันสมัยกำลังอัปเดตเป็นประสบการณ์การใช้งาน Yammer ใหม่และพร้อมใช้งานสำหรับผู้เช่าที่มีการวางเป้าหมาย GA ไวร์ได้เริ่มต้นแล้ว ฟีเจอร์ใหม่รวมถึงความสามารถในการเริ่มต้นการสนทนากับโพสต์ใดๆ (คำถาม, การสำรวจ, การสรรเสริญ) และทำเครื่องหมายคำตอบที่ดีที่สุดโดยตรงจาก SharePoint สำหรับข้อมูลเพิ่มเติมให้ดูที่[ข้อกำหนดและคำถามที่ถามบ่อยของลูกค้า Yammer ใหม่](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)

 เมื่อต้องการทำความเข้าใจเกี่ยวกับ web part และการกำหนดค่าที่เหมาะกับคุณให้ดูที่การ[ใช้ web part สำหรับ Yammer ใน SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)  

**การใช้ web part กับ SharePoint Server**  

Web part สามารถใช้ได้ในหน้าสมัยใหม่และคลาสสิกภายในสภาพแวดล้อมภายในองค์กร

- สำหรับข้อมูลเพิ่มเติมเกี่ยวกับหน้าสมัยใหม่ให้ดู[ที่เพิ่มตัวดึงข้อมูล Yammer ลงในหน้าใหม่ใน SharePoint Server ๒๐๑๙](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019) 
- สำหรับข้อมูลเพิ่มเติมเกี่ยวกับหน้าคลาสสิกให้ดู[ที่เพิ่มตัวดึงข้อมูล Yammer ลงในหน้าคลาสสิกใน SharePoint server ๒๐๑๓, ๒๐๑๖และ๒๐๑๙](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)

**ฝัง Yammer**  

ใช้เครื่องมือการกำหนดค่าฝังเพื่อทดสอบการใช้งานฝัง การอัปเดตในอนาคตเพื่อฝังจะเปิดใช้งานประสบการณ์การใช้งาน Yammer ใหม่ สำหรับข้อมูลเพิ่มเติมให้ดูที่ [เครื่องมือการกำหนดค่าฝัง](https://aka.ms/YammerEmbedConfigureTool)ตัวของ Yammer เมื่อต้องการทำความเข้าใจเกี่ยวกับคอมโพเนนต์ฝังตัวของ Yammer ให้ดูที่[ฝังตัวดึงข้อมูล](https://aka.ms/YammerDevDocs)

**ปัญหาที่ทราบและข้อจำกัด**

- รหัสกลุ่มจะไม่พร้อมใช้งานจาก Url Yammer ใหม่ซึ่งมีการเปลี่ยนแปลง สลับกลับไปยังโหมดคลาสสิกเพื่อรับ Id ของกลุ่มหรือ Id อื่นๆจาก Url
- โดเมนแบบกำหนดเอง (โต๊ะทำงาน) ไม่ได้รับการสนับสนุน
- Yammer ฝังตัวไม่ได้รับการปรับให้เหมาะสมสำหรับอุปกรณ์เคลื่อนที่ ใช้หน้าสมัยใหม่ที่มี web part สำหรับการสนทนา Yammer สำหรับประสบการณ์การใช้งานที่ดีที่สุด
- ธีมแบบกำหนดเองจะมีผลต่อลักษณะที่ปรากฏและการใช้งาน web part การสนทนา Yammer เปิดกรณีสนับสนุนเพื่อรายงานปัญหา