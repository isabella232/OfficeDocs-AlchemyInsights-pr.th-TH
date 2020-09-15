---
title: เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713149"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint

ทำตามขั้นตอนการแก้ไขปัญหาเหล่านี้เมื่อเนื้อหาที่คาดไว้ไม่ปรากฏในผลลัพธ์การค้นหา:
  
1. ตรวจสอบว่า **ไซต์** ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าเพื่ออนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา ทำตามขั้นตอนใน[แสดงเนื้อหาบนไซต์ในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. ตรวจสอบว่า **ราย** การหรือ **ไลบรารี** ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา ทำตามขั้นตอนใน[แสดงเนื้อหาจากรายการหรือไลบรารีในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. ตรวจสอบว่าหน้าเอกสารหรือเค้าโครงเพจที่กำหนดเองได้รับการเผยแพร่เป็น **เวอร์ชันหลัก** ทำตามขั้นตอนที่3ในการ[ค้นหาไม่ส่งกลับผลลัพธ์ทั้งหมดใน SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525)

4. ตรวจสอบว่าผู้ใช้มี **สิทธิ์** ในการดูเนื้อหา ทำตามขั้นตอนในการ[ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. ถ้า schema การค้นหาได้รับการเปลี่ยนแปลงโดยการเพิ่มคุณสมบัติที่มีการจัดการใหม่ด้วยการแก้ไขคุณสมบัติที่มีการจัดการหรือโดยการเอาคุณสมบัติที่มีการจัดการออกแล้วการร้องขอการตระเวนและการทำดัชนีใหม่จะต้องใช้ ทำ**ดัชนีเนื้อหาอีกครั้ง**โดยทำตามขั้นตอนในการ[ร้องขอการตระเวนด้วยตนเองและการทำดัชนีของไซต์ใหม่ไลบรารีหรือรายการ](https://docs.microsoft.com/sharepoint/crawl-site-content) การดำเนินการนี้อาจใช้เวลาสักครู่รอ24ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์อีกครั้ง

สำหรับข้อมูลเพิ่มเติมให้ดู [ที่เปิดใช้งานเนื้อหาบนไซต์เพื่อให้สามารถค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable)ได้ 
  
