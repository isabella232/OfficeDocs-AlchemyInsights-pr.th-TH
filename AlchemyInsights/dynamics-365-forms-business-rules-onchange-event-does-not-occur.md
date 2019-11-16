---
title: Dynamics ๓๖๕กฎทางธุรกิจของฟอร์ม-กฎทางธุรกิจไม่ยิงสำหรับฟอร์ม
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769358"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>เหตุการณ์ OnChange ไม่เกิดขึ้นถ้าฟิลด์ถูกเปลี่ยนโดยทางโปรแกรม

เหตุการณ์*OnChange*ไม่เกิดขึ้นถ้าเขตข้อมูลถูกเปลี่ยนโดยทางโปรแกรมโดยใช้*แอตทริบิวต์* เมธอด[Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ถ้าคุณต้องการจัดการเหตุการณ์สำหรับเหตุการณ์*OnChange*ที่จะเรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้*formcontext. ข้อมูลวิธี fireOnchange แอตทริบิวต์ของเอนทิตี* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)ในรหัสของคุณ

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
