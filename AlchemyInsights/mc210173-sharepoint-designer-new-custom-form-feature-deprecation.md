---
title: MC210173 - SharePointการเลิกใช้ฟีเจอร์ฟอร์มแบบSharePoint Designer ใหม่
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
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077699"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePointการเลิกใช้ฟีเจอร์ฟอร์มแบบSharePoint Designer ใหม่

เราได้ระบุปัญหาที่มีผลกระทบต่อฟังก์ชันการSharePoint Designer ในการสร้างฟอร์ม[แบบSharePoint](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)ภายใน Online หลังจากระมัดระวังการใช้ความระมัดระวัง เราได้กําหนดว่า ไม่มีการแก้ไขที่ทราบแล้วของปัญหานี้ และได้เลือกที่จะปิดใช้งานฟีเจอร์การสร้างฟอร์มแบบกําหนดเองได้อย่างมีประสิทธิภาพตั้งแต่ 3:00 น. UTC ในวันเสาร์ 25 เมษายน 2020 การเปลี่ยนแปลงนี้จะไม่ส่งผลกระทบต่อความสามารถในการแก้ไขฟอร์มที่สร้างไว้ก่อนหน้านี้หรือฟีเจอร์อื่นๆ ที่มีอยู่แล้วใน SharePoint Online Designer

หลังจากการเปลี่ยนแปลงนี้แล้ว ผู้ใช้อาจได้รับข้อผิดพลาด: "ไม่สามารถบันทึกการเปลี่ยนแปลงรายการไปยังเซิร์ฟเวอร์ได้" เมื่อสร้างฟอร์มใหม่

ผู้ใช้ที่ใช้ประโยชน์ก่อนหน้านี้SharePoint Designer ในการสร้างฟอร์มแบบปรับแต่งเองจะสามารถใช้[PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)เพื่อจุดประสงค์นี้แทนได้

PowerApps เป็นเครื่องมือที่ง่ายและรวดเร็วที่ช่วยให้ผู้ใช้สามารถดําเนินการในประสบการณ์การใช้งานที่ทันสมัยของ SharePoint Online เพื่อสร้างและแก้ไขฟอร์มแบบSharePointรายการและไลบรารีเอกสารได้จากหน้าต่างเบราว์เซอร์ PowerApps ไม่ต้องมีการเขียนโค้ดความรู้แบบดั้งเดิมหรือการดาวน์โหลดแอปเพิ่มเติมใดๆ เช่น InfoPath

**หมายเหตุ**: SharePointผู้ใช้ Online Classic จะต้องสลับไปยังประสบการณ์การใช้งานที่ทันสมัยชั่วคราวเพื่อเข้าถึงและใช้ PowerApps แม้ว่า ฟอร์มแบบปรับแต่งเองทั้งหมดที่สร้างขึ้นใน PowerApps จะสามารถเข้าถึงได้SharePointประสบการณ์การใช้งาน Online Online ของผู้ใช้
