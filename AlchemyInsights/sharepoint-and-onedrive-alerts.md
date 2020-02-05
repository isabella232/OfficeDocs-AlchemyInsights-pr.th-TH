---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771234"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive

- ก่อนอื่นให้ตรวจสอบโฟลเดอร์ขยะหรือสแปมในอีเมลของคุณ
- ถ้าการ**แจ้งเตือนทั้งหมดจากแฟ้มหรือไลบรารีหลายล่าช้า**โปรดเยี่ยมชม[แดชบอร์ดความสมบูรณ์ของบริการ](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)เพื่อตรวจสอบคำแนะนำ/เหตุการณ์ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหานี้อาจมีความสามารถในการแจ้งเตือนของ SharePoint หรือล่าช้าในอีเมผ่าน Exchange นอกจากนี้โปรดทราบว่าอีเมลอื่นๆจะถูกส่ง—ถ้าไม่มีปัญหาอาจมีความล่าช้าในอัตราแลกเปลี่ยน
- ถ้าการ**แจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุไม่ได้ถูกส่ง**ให้พยายามลบและสร้างใหม่ ดูที่[จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0)เพื่อสร้างการแจ้งเตือนใหม่

> [!NOTE]
> - ไม่สามารถส่งข้อความแจ้งเตือนไปยังกลุ่มการแจกจ่าย สนับสนุนเฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้น
> - คุณไม่สามารถกำหนดแม่แบบอีเมลแจ้งเตือนเองได้ คุณต้องใช้ลำดับงานของ Microsoft Flow หรือตัวออกแบบของ SharePoint เพื่อให้บรรลุเหล่านั้น
