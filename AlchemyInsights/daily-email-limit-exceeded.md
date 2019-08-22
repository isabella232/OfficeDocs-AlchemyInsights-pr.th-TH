---
title: ประจำวันอีเมลเกินขีดจำกัด ลำดับงานหยุดการทำงาน
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514492"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>อีเมลของรายวันเกินขีดจำกัด ลำดับงานหยุดการทำงาน

อาจได้รับข้อผิดพลาดนี้ในสถานการณ์ต่อไปนี้:

- คุณมีลำดับงานใน SharePoint แบบออนไลน์ที่กำลังใช้ SharePoint 2010 หรือชนิดแพลตฟอร์มเวิร์กโฟลว์ SharePoint 2013 ในส่วน
- เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความอีเมลที่กำหนดเองแก่ผู้ใช้มากกว่า 200 ในแต่ละครั้ง ผู้รับมากกว่า 10000 ต่อวัน หรือข้อความมากกว่า 30 ต่อนาที
- เมื่อคุณเรียกใช้เวิร์กโฟลว์ ไม่ได้ส่งข้อความอีเมล และคุณสังเกตเห็นลักษณะการทำงานต่อไปนี้:
    - สำหรับเวิร์กโฟลว์โดยใช้ชนิดแพลตฟอร์ม SharePoint 2013 คุณเรียกดูไปยังหน้า**สถานะลำดับงาน** บนหน้าสถานะลำดับงาน**ภายในสถานะ**ถูกตั้งค่าเป็น**เริ่มต้นแล้ว**และ**ไม่สามารถส่งไปยังผู้รับ**ที่แสดงข้อมูลบอลลูน

เมื่อต้องการหลีกเลี่ยงปัญหานี้ กำหนดค่าเวิร์กโฟลว์ของคุณจะส่งข้อความอีเมลโดยไม่เกิน[ขีดจำกัดผู้ส่งอัตราแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่น ใช้ในเวิร์กโฟลว์หยุดชั่วคราว ส่งอีเมลไปยังกลุ่ม Office 365 กลุ่มการแจกจ่าย หรือกลุ่มรักษาความปลอดภัยจดหมายที่เปิดใช้งาน หรือส่งข้อความไปยังผู้รับที่น้อยกว่า 200 ในแต่ละครั้ง


สำหรับข้อมูลเพิ่มเติม ให้ดู[บท](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ความต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และขั้นตอน](https://flow.microsoft.com/blog/sharepoint-and-flow/) 