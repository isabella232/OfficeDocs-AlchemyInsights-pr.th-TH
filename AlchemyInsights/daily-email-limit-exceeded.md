---
title: เกินขีดจำกัดของ email รายวัน เวิร์กโฟลว์ถูกระงับ
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053136"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>เกินขีดจำกัดของ email รายวัน เวิร์กโฟลว์ถูกระงับ

ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:

- คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ SharePoint ๒๐๑๐หรือ SharePoint ๒๐๑๓ชนิดแพลตฟอร์มเวิร์กโฟลว์
- เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความเมลแบบกำหนดเองไปยังผู้ใช้มากกว่า๒๐๐ในแต่ละครั้งมากกว่า๑๐,๐๐๐ผู้รับต่อวันหรือมากกว่า30ข้อความต่อนาที
- เมื่อคุณเรียกใช้เวิร์กโฟลว์ข้อความทางเมลไม่ถูกส่งและคุณสังเกตเห็นลักษณะการทำงานต่อไปนี้:
    - สำหรับเวิร์กโฟลว์โดยใช้ชนิดแพลตฟอร์ม SharePoint ๒๐๑๓คุณเรียกดูไปยังหน้า**สถานะลำดับงาน** บนหน้าสถานะลำดับงาน**สถานะภายใน**ถูกตั้งค่าเป็น**เริ่มต้น**และบอลลูนข้อมูลแสดง**ไม่สามารถส่งไปยังผู้รับ**

การกำหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความทางเมลโดยไม่เกิน[ขีดจำกัดผู้ส่งแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่นใช้หยุดการทำงานในเวิร์กโฟลว์ให้ส่งจดหมายไปยังกลุ่ม Office ๓๖๕, กลุ่มการแจกจ่ายหรือกลุ่มรักษาความปลอดภัยที่เปิดใช้งานเมลหรือส่งข้อความไปยังผู้รับน้อยกว่า๒๐๐ในแต่ละครั้ง


สำหรับข้อมูลเพิ่มเติมให้ดู[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 