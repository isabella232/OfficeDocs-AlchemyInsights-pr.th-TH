---
title: SharePointการแจ้งเตือนยังไม่ได้ส่ง
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
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957920"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePointการแจ้งเตือนยังไม่ได้ส่ง

โปรดตรวจสอบโฟลเดอร์ อีเมลขยะ ในอีเมลของคุณ เนื่องจากบางครั้งการแจ้งเตือนอาจอยู่ที่นั่น

ระบุว่า **การแจ้งเตือนทั้งหมดจะไม่ถูกส่งหรือ****ส่งการแจ้งเตือนแต่ละรายการ** จากไฟล์หรือไลบรารีที่ระบุ

- **การแจ้งเตือนแต่ละรายการจะไม่ถูกส่ง**: ถ้าการแจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่ระบุไม่ได้ถูกส่งมา คุณสามารถพยายามที่จะลบและสร้างใหม่ได้ [ให้ดูที่ จัดการ ดู หรือลบSharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)การแจ้งเตือน เพื่อสร้างการแจ้งเตือนใหม่
- **การแจ้งเตือนทั้งหมดจะไม่ถูกส่ง**: ถ้าการแจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการไม่ได้ถูกส่งให้ไปที่แดชบอร์ดสถานภาพบริการเพื่อตรวจสอบที่ปรึกษา [](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)/เหตุการณ์ใดๆ ที่อาจเกิดขึ้นกับSharePointหรือExchangeบริการ ปัญหาอาจเกิดจากความสามารถในการSharePointการแจ้งเตือนหรือความล่าช้าในอีเมลผ่านExchangeการแจ้งเตือน นอกจากนี้ยังควรทราบว่ามีการส่งอีเมลอื่นหรือไม่ และถ้าไม่ อาจเกิดปัญหานี้ขึ้นExchangeความล่าช้าได้

ถามที่ถามบ่อยเกี่ยวกับการแจ้งเตือน:

- ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่าย เฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน
- คุณไม่สามารถปรับแต่งเทมเพลตอีเมลการแจ้งเตือนได้ คุณต้องใช้ Microsoft FLOW หรือเวิร์กโฟลว์ SharePoint Designer เพื่อให้บรรลุเป้าหมายเหล่านั้นได้

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง

ต้องการMicrosoft Flowใน SharePoint Online ใช่ไหม

- [สร้างFlow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePointและFlow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
