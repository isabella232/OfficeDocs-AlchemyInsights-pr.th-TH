---
title: ไม่ได้รับการแจ้งเตือน SharePoint และ OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205561"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>ไม่ได้รับการแจ้งเตือน SharePoint และ OneDrive

ก่อนอื่นให้ตรวจสอบโฟลเดอร์ขยะหรือสแปมใน email ของคุณ

จากนั้นตรวจสอบว่าการ**แจ้งเตือนทั้งหมดจะไม่ถูกส่ง**หรือถ้าไม่มี**การส่งการแจ้งเตือนแต่ละรายการ**จากแฟ้มหรือไลบรารีเฉพาะ

- ถ้า**ไม่มีการส่งการแจ้งเตือนทั้งหมดจากแฟ้มหรือไลบรารีหลายรายการ**ให้ไปที่[แดชบอร์ดความสมบูรณ์ของบริการ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)เพื่อตรวจสอบคำแนะนำ/เหตุการณ์ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหานี้อาจจะมีความสามารถในการแจ้งเตือนของ SharePoint หรือล่าช้าในการใช้งานในเมลผ่านการแลกเปลี่ยน นอกจากนี้โปรดทราบว่าจะมีการจัดส่งเมลอื่น—ถ้าไม่มีปัญหาอาจเกิดขึ้นกับความล่าช้าของอัตราแลกเปลี่ยน
- ถ้า**ไม่มีการส่งการแจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุ**ให้พยายามลบและสร้างข้อความนั้นใหม่ ดู[จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)เพื่อสร้างการแจ้งเตือนใหม่

> [!NOTE]
> - ไม่สามารถส่งข้อความแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้ สนับสนุนเฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้น
> - คุณไม่สามารถกำหนดเทมเพลตอีเมลแจ้งเตือนได้ คุณต้องใช้ Microsoft Flow หรือลำดับงานของ SharePoint Designer เพื่อให้บรรลุเป้าหมายเหล่านั้น
