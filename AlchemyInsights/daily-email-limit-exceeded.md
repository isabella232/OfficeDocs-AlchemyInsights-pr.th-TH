---
title: เกินขีดจำกัดของอีเมลในชีวิตประจำวัน เวิร์กโฟลว์ถูกหยุดชั่วคราว
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
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731582"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>เกินขีดจำกัดของอีเมลในชีวิตประจำวัน เวิร์กโฟลว์ถูกหยุดชั่วคราว

ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:

- คุณมีเวิร์กโฟลว์ใน SharePoint Online ที่กำลังใช้ชนิดของแพลตฟอร์มเวิร์กโฟลว์ sharepoint ๒๐๑๐หรือ SharePoint ๒๐๑๓
- เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความอีเมลที่กำหนดเองไปยังผู้ใช้มากกว่า๒๐๐คนในเวลามากกว่าผู้รับ๑๐,๐๐๐รายต่อวันหรือมากกว่า30ข้อความต่อนาที
- เมื่อคุณเรียกใช้เวิร์กโฟลว์จะไม่มีการส่งข้อความอีเมลและคุณสังเกตเห็นลักษณะการทำงานต่อไปนี้:
    - สำหรับเวิร์กโฟลว์ที่ใช้ชนิดแพลตฟอร์ม SharePoint ๒๐๑๓คุณเรียกดูหน้า**สถานะเวิร์กโฟลว์** บนหน้าสถานะเวิร์กโฟลว์จะมีการตั้งค่า **สถานะภายใน** เป็น **เริ่มต้น**และบอลลูนข้อมูลจะ **ไม่สามารถส่งไปยังผู้รับ**ได้

เมื่อต้องการแก้ไขปัญหานี้ให้กำหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่เกิน[ขีดจำกัดผู้ส่ง Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่นใช้หยุดชั่วคราวในเวิร์กโฟลว์ส่งอีเมลไปยังกลุ่ม Microsoft ๓๖๕กลุ่มการแจกจ่ายหรือกลุ่มการรักษาความปลอดภัยที่เปิดใช้งานจดหมายหรือส่งข้อความให้น้อยกว่าผู้รับ๒๐๐ในแต่ละครั้ง


สำหรับข้อมูลเพิ่มเติมให้ดู [บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 