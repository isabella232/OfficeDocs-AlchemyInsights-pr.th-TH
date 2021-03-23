---
title: ตัวดึงข้อมูลใน Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003219"
- "9666"
ms.openlocfilehash: d933c2b7fa73d6ab1fd91a452ed5736d084cdd18
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038136"
---
# <a name="feeds-in-yammer"></a>ตัวดึงข้อมูลใน Yammer

**ตัวดึงข้อมูล**

Yammer ใหม่เปิดตัว [ฟีดหน้าแรก](https://support.microsoft.com/office/what-s-in-the-yammer-home-feed-8fff52dd-5b38-468c-b963-fa4c6a4f9254)ใหม่ คุณสามารถอ่านเพิ่มเติมว่า [มีอะไรใหม่ในฟีดนี้ ซึ่ง](https://techcommunity.microsoft.com/t5/yammer-blog/yammer-discovery-what-is-in-my-feed/ba-p/1596230) ออกแบบมาเพื่อแสดงเนื้อหาจากชุมชนของคุณและช่วยให้คุณค้นพบเนื้อหาใหม่ การโฮเวอร์เหนือตัวเลือก ตัวดึงข้อมูลหน้าแรก จะเปิดใช้งานเมนูที่สามารถเข้าถึงมุมมอง การสนทนาทั้งหมด ได้ การอัปเดตในอนาคตของตัวดึงข้อมูลอาจส่งเนื้อหาจากแหล่งเพิ่มเติมมาภายในชุดโปรแกรม Microsoft 365

Yammer แบบคลาสสิก [มีฟีด](https://support.microsoft.com/office/what-s-in-the-yammer-discovery-feed-28ba9a79-2bde-4e7c-8420-db2296c3ca49) การค้นพบที่ไม่ได้ขั้นสูงเกี่ยวกับวิธีการระบุเนื้อหาให้คุณ ตัวเลือกในการสลับไปยังตัวดึงข้อมูลทั้งหมดและตัวดึงข้อมูลที่ติดตามจะพร้อมใช้งานที่ด้านบนของโฮมเพจ

ตัวดึงข้อมูล Yammer ยังสามารถถูกรวมไว้ในไซต์ SharePoint โดยใช้[การสนทนา Yammer และ Web Part ไฮไลต์](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)

**การโพสต์ปัญหา**

ควรสามารถโพสต์ไปยัง Yammer ได้หลายวิธี ต่อไปนี้คือปัญหาทั่วไปที่ผู้ใช้อาจประสบ:

- ผู้ดูแลระบบได้ [จํากัดการโพสต์การสนทนาใหม่ใน](https://support.microsoft.com/office/restrict-all-company-posts-in-yammer-3219d2ae-db15-4c9f-9dd2-28559ae39a97) All Company นี่คือข้อจํากัดที่ผู้ดูแลระบบจะต้องเอาออกเพื่ออนุญาตให้ผู้ใช้ทั่วไปสามารถโพสต์ได้
- การเป็นสมาชิกของชุมชนไม่ได้รับการซิงค์อย่างถูกต้อง ตัวอย่างเช่น ผู้ใช้เป็นสมาชิกของชุมชนใน Yammer แต่ไม่ใช่กลุ่ม Microsoft 365 ที่เชื่อมต่อกับ SharePoint Online รอให้การซิงค์การเป็นสมาชิกเสร็จสมบูรณ์ของกลุ่มที่มีขนาดใหญ่มากอาจใช้เวลาถึง 24 ชั่วโมง
- การอัปเดตโค้ดจาก CDN ไม่สามารถโหลดได้อย่างถูกต้อง การล้างแคชและคุกกี้ของเบราว์เซอร์มักจะแก้ไขปัญหานี้
