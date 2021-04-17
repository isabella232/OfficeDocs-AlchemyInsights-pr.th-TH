---
title: MC210173 - การเลิกใช้ฟีเจอร์ฟอร์มแบบปรับแต่งเองของ SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831825"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - การเลิกใช้ฟีเจอร์ฟอร์มแบบปรับแต่งเองของ SharePoint Designer

เราได้ระบุปัญหาที่มีผลกระทบต่อฟังก์ชันการใช้ฟังก์ชัน SharePoint Designer ในการสร้าง [ฟอร์มแบบปรับแต่งเอง](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) ภายใน SharePoint Online หลังจากระมัดระวังการใช้ความระมัดระวัง เราได้กําหนดว่า ไม่มีการแก้ไขที่ทราบแล้วของปัญหานี้ และได้เลือกที่จะปิดใช้งานฟีเจอร์การสร้างฟอร์มแบบกําหนดเองได้อย่างมีประสิทธิภาพตั้งแต่ 3:00 น. UTC ในวันเสาร์ 25 เมษายน 2020 การเปลี่ยนแปลงนี้จะไม่ส่งผลกระทบต่อความสามารถในการแก้ไขฟอร์มที่สร้างไว้ก่อนหน้านี้หรือฟีเจอร์ที่มีอยู่อื่นๆ ใน SharePoint Online Designer

หลังจากการเปลี่ยนแปลงนี้แล้ว ผู้ใช้อาจได้รับข้อผิดพลาด: "ไม่สามารถบันทึกการเปลี่ยนแปลงรายการไปยังเซิร์ฟเวอร์ได้" เมื่อสร้างฟอร์มใหม่

ผู้ใช้ที่ใช้ SharePoint Designer มาก่อนหน้านี้เพื่อสร้างฟอร์มแบบปรับแต่งเองจะสามารถใช้ [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) เพื่อจุดประสงค์นี้แทนได้

PowerApps เป็นเครื่องมือที่ง่ายและมีประสิทธิภาพที่ช่วยให้ผู้ใช้สามารถดําเนินการในประสบการณ์ที่ทันสมัยของ SharePoint Online เพื่อสร้างและแก้ไขฟอร์มแบบปรับแต่งเองในรายการ SharePoint และไลบรารีเอกสารได้จากหน้าต่างเบราว์เซอร์ PowerApps ไม่ต้องมีการเขียนโค้ดความรู้แบบดั้งเดิมหรือการดาวน์โหลดแอปเพิ่มเติมใดๆ เช่น InfoPath

**หมายเหตุ**: ผู้ใช้ SharePoint Online Classic จะต้องสลับไปยังประสบการณ์การใช้งานที่ทันสมัยชั่วคราวเพื่อเข้าถึงและใช้ PowerApps แม้ว่า ฟอร์มแบบปรับแต่งเองทั้งหมดที่สร้างขึ้นใน PowerApps จะสามารถเข้าถึงได้โดยผู้ใช้ประสบการณ์การใช้งาน SharePoint Online แบบคลาสสิก
