---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785684"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive

- ก่อนอื่นให้ตรวจสอบโฟลเดอร์อีเมลขยะหรือสแปมในอีเมลของคุณ
- ถ้าการ **แจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการมีความล่าช้า**ให้ไปที่ [แดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth) เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหานี้อาจเกิดขึ้นกับความสามารถในการแจ้งเตือนของ SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange โปรดสังเกตว่าจะมีการส่งอีเมลอื่นๆหรือไม่ถ้าไม่มีปัญหาเกิดขึ้นกับความล่าช้าของ Exchange
- ถ้าการ **แจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่ระบุไม่ได้รับการส่ง**ให้พยายามลบและสร้างใหม่ ดู [จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่

> [!NOTE]
> - ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้ เฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน
> - คุณไม่สามารถกำหนดแม่แบบอีเมลการแจ้งเตือนเองได้ คุณต้องใช้ Microsoft Flow หรือเวิร์กโฟลว์ตัวออกแบบของ SharePoint เพื่อให้บรรลุเป้าหมายเหล่านั้น
