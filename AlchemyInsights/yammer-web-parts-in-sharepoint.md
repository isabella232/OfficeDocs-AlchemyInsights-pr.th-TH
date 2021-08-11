---
title: Yammer Web Part ใน SharePoint
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
ms.openlocfilehash: a252dab703e639c7c11fe6aead1db04aeecfe54bc6d52bcd4a28433aed4701d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970350"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Yammer Web Part ใน SharePoint

Yammer การสนทนาและการYammerเน้นที่ Web Part จะช่วยเพิ่มประสิทธิภาพการร่วมมือกันบนหน้าSharePointสมัยใหม่และแบบคลาสสิก ดูข้อมูลเพิ่มเติมได้ที่ การYammer[และ](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)[Yammerไฮไลต์](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)    

Web part Yammer Conversations ที่ทันสมัยได้รับการอัปเดตเป็นประสบการณ์การใช้งานYammerใหม่และพร้อมใช้งานในผู้เช่าการเผยแพร่ที่เป้าหมาย เริ่มต้นการเริ่มใช้งาน GA แล้ว ฟีเจอร์ใหม่รวมถึงความสามารถในการเริ่มการสนทนากับโพสต์ต่างๆ (คําถาม โพล คําชมเชย) และเพื่อเขียนเครื่องหมายคําตอบที่ดีที่สุดโดยตรงจากSharePointของคุณ For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).

 เมื่อต้องการเข้าใจว่า Web Part ใดและการกําหนดค่าที่เหมาะสมให้คุณ ให้ดูที่ Yammer [Web Part SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)  

**การใช้ Web Part กับ SharePoint Server**  

Web Part สามารถใช้ได้ในหน้าสมัยใหม่และแบบคลาสสิกภายในสภาพแวดล้อมภายในองค์กร

- For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Yammer Embed**  

ใช้เครื่องมือ การกําหนดค่าที่ฝัง เพื่อทดสอบ การฝังการใช้งาน การอัปเดตในอนาคตเป็น ฝัง จะเปิดใช้งานประสบการณ์Yammerใหม่ For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool). เมื่อต้องการเข้าใจคอมโพเนนต์ Yammer ฝัง ดีขึ้น ให้ดูที่[ฝังตัว](https://aka.ms/YammerDevDocs)ดึงข้อมูล

**ปัญหาที่ทราบและข้อจํากัด**

- ไม่มีรหัสกลุ่มจาก URL Yammerใหม่ที่มีการเปลี่ยนแปลง สลับกลับไปยังโหมดคลาสสิกเพื่อรับรหัสกลุ่มหรือรหัสอื่นๆ จาก URL
- โดเมนแบบปรับแต่งเอง (ไม่รองรับ)
- Yammer ฝังไม่ได้รับการปรับให้เหมาะสมกับอุปกรณ์เคลื่อนที่ ใช้หน้าสมัยใหม่ด้วย web part Yammer Conversations เพื่อประสบการณ์การใช้งานที่ดีที่สุด
- ธีมแบบปรับแต่งเองอาจส่งผลต่อลักษณะที่ปรากฏและการYammer Web Part การสนทนา เปิดกรณีสนับสนุนเพื่อรายงานปัญหา