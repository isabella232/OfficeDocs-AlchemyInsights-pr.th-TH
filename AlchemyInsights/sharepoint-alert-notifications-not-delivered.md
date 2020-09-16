---
title: การแจ้งเตือนการแจ้งเตือนของ SharePoint ไม่ถูกส่ง
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751262"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>การแจ้งเตือนการแจ้งเตือนของ SharePoint ไม่ถูกส่ง

โปรดตรวจสอบโฟลเดอร์อีเมลขยะในอีเมลของคุณในบางครั้งการแจ้งเตือนอาจไปที่นั่น

กำหนดว่าการ **แจ้งเตือนทั้งหมดจะไม่ถูกส่ง** หรือถ้า **การแจ้งเตือนแต่ละรายการ** จากไฟล์หรือไลบรารีที่ระบุไม่ได้ถูกส่ง

- การ**แจ้งเตือนแต่ละรายการจะไม่ถูกส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่เฉพาะเจาะจงคุณสามารถพยายามลบและสร้างใหม่ได้ ดู [จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่
- การ**แจ้งเตือนทั้งหมดจะไม่ถูกส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการให้ไปที่[แดชบอร์ดสถานภาพบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหานี้อาจเกิดจากความสามารถในการแจ้งเตือนของ SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange นอกจากนี้ยังมีความสำคัญในการสังเกตว่าอีเมลอื่นๆกำลังถูกส่งและถ้าไม่มีปัญหาเกิดขึ้นกับ Exchange ล่าช้า

คำถามที่ถามบ่อยเกี่ยวกับการแจ้งเตือน:

- ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายเฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน
- คุณไม่สามารถกำหนดแม่แบบอีเมลการแจ้งเตือนเองได้ คุณจำเป็นต้องใช้เวิร์กโฟลว์ของ Microsoft FLOW หรือ SharePoint Designer เพื่อให้บรรลุเป้าหมายเหล่านั้น

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง

ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่

- [สร้างขั้นตอน](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint และการไหล](https://flow.microsoft.com//blog/sharepoint-and-flow/)
