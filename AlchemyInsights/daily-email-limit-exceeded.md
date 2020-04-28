---
title: เกินขีดจํากัดของอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ
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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908723"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>เกินขีดจํากัดอีเมลรายวันแล้ว เวิร์กโฟลว์ถูกระงับ

ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:

- คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ SharePoint 2010 หรือ SharePoint 2013
- เวิร์กโฟลว์ถูกกําหนดค่าให้ส่งข้อความอีเมลแบบกําหนดเองไปยังผู้ใช้มากกว่า 200 คนในแต่ละครั้ง
- เมื่อคุณเรียกใช้เวิร์กโฟลว์ ข้อความอีเมลที่จะไม่ส่ง และคุณสังเกตเห็นลักษณะการทํางานต่อไปนี้:
    - สําหรับเวิร์กโฟลว์ที่ใช้ชนิดแพลตฟอร์ม SharePoint 2013 คุณเรียกดูไปยังหน้า**สถานะเวิร์กโฟลว์** บนหน้า สถานะเวิร์กโฟลว์**สถานะภายใน**ถูกตั้งค่าเป็น**เริ่มต้น**แล้ว และบอลลูนข้อมูลจะแสดง**ไม่สามารถส่งไปยังผู้รับ**ได้

เมื่อต้องการหลีกเลี่ยงปัญหานี้ กําหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่เกิน[ขีดจํากัดผู้ส่งแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่น ใช้หยุดชั่วคราวในเวิร์กโฟลว์ ส่งอีเมลไปยังกลุ่ม Microsoft 365 กลุ่มการแจกจ่ายหรือกลุ่มรักษาความปลอดภัยที่เปิดใช้งานจดหมาย หรือส่งข้อความไปยังผู้รับน้อยกว่า 200 ในแต่ละครั้ง


สําหรับข้อมูลเพิ่มเติม ให้ดูที่[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และโฟลว์](https://flow.microsoft.com/blog/sharepoint-and-flow/) 