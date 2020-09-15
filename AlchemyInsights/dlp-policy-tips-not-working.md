---
title: เคล็ดลับนโยบาย DLP ไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679604"
---
# <a name="dlp-policy-tip-issues"></a>ปัญหาเกี่ยวกับเคล็ดลับนโยบาย DLP

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**เคล็ดลับนโยบาย DLP**

เมื่อใช้**นโยบาย DLP**ผู้ใช้สามารถได้รับการแจ้งให้ทราบเกี่ยวกับการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย** ผู้ดูแลระบบสามารถกำหนดค่าเคล็ดลับนโยบายในการแสดงในขณะที่ทดสอบนโยบาย DLP ของพวกเขาหรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้แบบเต็ม
  
เมื่อต้องการกำหนดค่าเคล็ดลับนโยบายในนโยบาย DLP ของคุณในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายในโหมดการบังคับใช้แบบเต็มให้ทำดังต่อไปนี้:
  
- ตรวจสอบให้แน่ใจว่ามีการ**เปิดใช้งาน**เคล็ดลับนโยบายในกฎ DLP โดยใช้ขั้นตอน[ต่อไปนี้](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)

- ตรวจสอบให้แน่ใจว่าเนื้อหาของคุณ**ตรงกับ**สิ่งที่จำเป็นต้อง**ใช้**ในการทริกเกอร์กฎที่ระบุไว้ในบทความนี้[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- เคล็ดลับนโยบายแสดงในทั้ง OWA และ Outlook อย่างไรก็ตามเมื่อใช้ **Outlook ๒๐๑๓หรือใหม่กว่า**คำแนะนำนโยบายจะแสดงเฉพาะภายใต้เงื่อนไขบางอย่าง เงื่อนไขเหล่านี้จะแสดงรายการที่นี่: เงื่อนไขที่ได้ [รับการสนับสนุนสำหรับ Outlook ๒๐๑๓หรือใหม่กว่าสำหรับการแสดงเคล็ดลับนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ให้ดูที่: [แสดงเคล็ดลับนโยบายสำหรับนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)
  