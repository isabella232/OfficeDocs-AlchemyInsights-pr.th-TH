---
title: อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670851"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive

ผู้ใช้อาจได้รับข้อความแบบ **อ่านอย่างเดียวสำหรับการบำรุงรักษา** เมื่อพยายามใช้ SharePoint หรือ OneDrive สำหรับสถานการณ์สมมติต่อไปนี้อย่างใดอย่างหนึ่ง 

-   กิจกรรมการบำรุงรักษาที่วางแผนไว้หรือที่ใช้งานอยู่  ตรวจสอบได้โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/messagecenter)
-   มีลำดับความสำคัญสูงเหตุการณ์บริการที่ใช้งานอยู่ที่อาจจะเกิดขึ้น ตรวจสอบคำแนะนำ/เหตุการณ์ใดก็ตามโดยการนำทางไปยัง[สถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)
-   สถานการณ์สมมติการกู้คืนอัตโนมัติสำหรับการฟื้นฟูที่อาจเกิดขึ้นได้เนื่องจากเหตุการณ์ที่ไม่คาดคิดบนเซิร์ฟเวอร์ที่อาจใช้เวลาน้อยกว่า30นาทีหรือดังนั้น 
    
    ไม่มีศูนย์ข้อความหรือข้อความสถานภาพบริการสำหรับการกลับมาเล็กน้อยเหล่านี้แต่คุณควรกลับมาใช้ตามปกติในเร็วๆนี้

ในบางโอกาสที่เราสังเกตว่าหนึ่งในสามสถานการณ์ที่แสดงไว้ด้านบนได้รับการคืนค่าและบริการได้รับการคืนค่าแล้วแต่แคชเบราว์เซอร์ผู้ใช้ยังไม่ได้รับการล้างข้อมูล

โปรดลองล้างแคชของเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์

1. ในเบราว์เซอร์ Microsoft Edge ของคุณให้เลือก**การตั้งค่า**แล้วเลือกความ**เป็นส่วนตัวและความปลอดภัย**
2. ภายใต้**ล้างการเรียกดู**ให้เลือก**เลือกสิ่งที่ต้องการล้าง**
3. เลือก**คุกกี้และข้อมูลเว็บไซต์ที่บันทึกไว้**แล้วเลือก**ล้าง**

>[!Note] 
> ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Mozilla Firefox หรือ Google Chrome

>[!Note] 
> อีกตัวเลือกหนึ่งคือการเปิดไซต์ SharePoint หรือ OneDrive ของคุณในหน้าต่างแบบ InPrivate ใหม่