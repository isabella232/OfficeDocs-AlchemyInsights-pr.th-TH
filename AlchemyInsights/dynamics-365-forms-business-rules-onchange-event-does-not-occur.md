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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529038"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>เหตุการณ์ OnChange ไม่เกิดขึ้นถ้าฟิลด์ถูกเปลี่ยนโดยทางโปรแกรม

เหตุการณ์*OnChange*ไม่เกิดขึ้นถ้าเขตข้อมูลถูกเปลี่ยนโดยทางโปรแกรมโดยใช้*แอตทริบิวต์* เมธอด[Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ถ้าคุณต้องการจัดการเหตุการณ์สำหรับเหตุการณ์*OnChange*ที่จะเรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้*formcontext. แอตทริบิวต์ของเอนทิตีข้อมูล* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)วิธีการในรหัสของคุณ

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
