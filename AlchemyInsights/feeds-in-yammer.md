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
ms.openlocfilehash: 855921cb5a1e84355a436a5a1f67a2518240fb804c14286f86e7f2fca306bb30
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117467"
---
# <a name="feeds-in-yammer"></a>ตัวดึงข้อมูลใน Yammer

**ตัวดึงข้อมูล**

เนื้อหาYammerเปิดตัว[ตัวดึงข้อมูลหลัก](https://support.microsoft.com/office/what-s-in-the-yammer-home-feed-8fff52dd-5b38-468c-b963-fa4c6a4f9254)ตัวใหม่ คุณสามารถอ่านเพิ่มเติมว่า [มีอะไรใหม่ในฟีดนี้](https://techcommunity.microsoft.com/t5/yammer-blog/yammer-discovery-what-is-in-my-feed/ba-p/1596230) ซึ่งออกแบบมาเพื่อแสดงเนื้อหาจากชุมชนของคุณและช่วยให้คุณค้นพบเนื้อหาใหม่ การโฮเวอร์เหนือตัวเลือก ตัวดึงข้อมูลหลัก จะเปิดใช้งานเมนูที่สามารถเข้าถึงมุมมอง การสนทนาทั้งหมด ได้ การอัปเดตในอนาคตของตัวดึงข้อมูลอาจดึงเนื้อหาจากแหล่งข้อมูลเพิ่มเติมMicrosoft 365ชุดโปรแกรม

ตัวควบคุมYammerจะมี[ฟีด](https://support.microsoft.com/office/what-s-in-the-yammer-discovery-feed-28ba9a79-2bde-4e7c-8420-db2296c3ca49)Discovery ซึ่งไม่ขั้นสูงเกี่ยวกับวิธีการระบุเนื้อหาให้คุณ ตัวเลือกในการสลับไปยังตัวดึงข้อมูล ทั้งหมด และ ที่ติดตาม จะพร้อมใช้งานที่ด้านบนของโฮมเพจ

Yammerเนื้อหาสรุปสามารถถูกรวมไว้ในSharePointไซต์ของคุณโดยใช้[Yammerและไฮไลต์ Web Part](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)

**ปัญหาการโพสต์**

คุณควรสามารถโพสต์Yammerได้หลายวิธี ต่อไปนี้คือปัญหาทั่วไปที่ผู้ใช้อาจพบเห็น:

- ผู้ดูแลระบบได้ [จํากัดการโพสต์การสนทนาใหม่ใน](https://support.microsoft.com/office/restrict-all-company-posts-in-yammer-3219d2ae-db15-4c9f-9dd2-28559ae39a97) บริษัททั้งหมด นี่คือข้อจํากัดที่ผู้ดูแลระบบจะต้องเอาออกเพื่ออนุญาตให้ผู้ใช้ทั่วไปสามารถโพสต์ได้
- การเป็นสมาชิกชุมชนไม่ได้ซิงค์อย่างถูกต้อง For example, a user is a member of a community in Yammer, but not the Microsoft 365 group connected to SharePoint Online. รอให้การซิงค์สมาชิกเสร็จสมบูรณ์ของกลุ่มที่มีขนาดใหญ่มากอาจใช้เวลาถึง 24 ชั่วโมง
- การอัปเดตโค้ดจาก CDN ไม่สามารถโหลดได้อย่างถูกต้อง การล้างแคชของเบราว์เซอร์และคุกกี้มักจะสามารถแก้ไขปัญหานี้ได้
