---
title: เกินขีดจํากัดอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580352"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>เกินขีดจํากัดอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ

ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:

- คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ชนิดแพลตฟอร์มลําดับงาน SharePoint 2010 หรือ SharePoint 2013
- เวิร์กโฟลว์ถูกกําหนดค่าให้ส่งข้อความอีเมลที่กําหนดเองไปยังผู้ใช้มากกว่า 200 รายในแต่ละครั้ง
- เมื่อคุณเรียกใช้เวิร์กโฟลว์ ข้อความอีเมลที่ไม่ได้ส่ง และคุณสังเกตเห็นลักษณะการทํางานต่อไปนี้:
    - สําหรับเวิร์กโฟลว์ที่ใช้ชนิดแพลตฟอร์ม SharePoint 2013 คุณเรียกดูไปยังหน้า**สถานะเวิร์กโฟลว์** บนหน้า สถานะเวิร์กโฟลว์**สถานะภายใน**จะถูกตั้งค่าเป็น**เริ่มต้น**แล้วบอลลูนข้อมูลจะแสดง**ไม่สามารถส่งไปยังผู้รับ**ได้

เมื่อต้องการหลีกเลี่ยงปัญหานี้ ให้กําหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่มีการ[เกินขีดจํากัดของผู้ส่ง Exchange แบบออนไลน์](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่น ใช้การหยุดชั่วคราวในเวิร์กโฟลว์ ส่งอีเมลไปยังกลุ่ม Microsoft 365 กลุ่มการแจกจ่ายหรือจดหมายที่เปิดใช้งานกลุ่มรักษาความปลอดภัย หรือส่งข้อความไปยังผู้รับน้อยกว่า 200 ครั้ง


สําหรับข้อมูลเพิ่มเติม ให้ดู[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [การไหลและจุด](https://flow.microsoft.com/blog/sharepoint-and-flow/) 