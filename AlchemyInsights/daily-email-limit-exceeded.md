---
title: เกินขีดจํากัดอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914670"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>เกินขีดจํากัดอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ

คุณอาจได้รับข้อผิดพลาดนี้ในสถานการณ์ต่อไปนี้:

- คุณมีเวิร์กโฟลว์ใน SharePoint Online ที่ใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ SharePoint 2010 หรือ SharePoint 2013
- เวิร์กโฟลว์ถูกกําหนดค่าให้ส่งข้อความอีเมลแบบกําหนดเองถึงผู้ใช้มากกว่า 200 คนในครั้งเดียวกัน ผู้รับมากกว่า 10,000 คนต่อวัน หรือมากกว่า 30 ข้อความต่อวัน
- เมื่อคุณเรียกใช้เวิร์กโฟลว์ ข้อความอีเมลนั้นจะไม่ถูกส่งไป และคุณจะสังเกตเห็นลักษณะการออนไลน์ต่อไปนี้
    - For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page. บนหน้า สถานะเวิร์กโฟลว์ สถานะ **ภายใน** ถูกตั้งค่า **เป็น** เริ่มแล้ว และบอลลูนข้อมูลจะแสดง **ไม่สามารถส่งไปยัง** ผู้รับได้

เมื่อต้องการแก้ไขปัญหานี้ให้กําหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่เกิน[ขีดExchange Onlineจํากัดผู้ส่ง](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) ตัวอย่างเช่น ใช้การหยุดชั่วคราวในเวิร์กโฟลว์ ส่งอีเมลไปยังกลุ่ม Microsoft 365 กลุ่มการแจกจ่ายหรือกลุ่มความปลอดภัยที่เปิดใช้งานจดหมาย หรือส่งข้อความไปยังผู้รับน้อยกว่า 200 คนในคราวเดียวกัน


หากต้องการข้อมูลเพิ่มเติม โปรดดู [บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
- [สร้างFlow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePointและFlow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 