---
title: กฎทางธุรกิจของ Dynamics 365 Forms - กฎธุรกิจไม่ firing for a Form
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947318"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>เหตุการณ์ OnChangs จะไม่เกิดขึ้นถ้าเขตข้อมูลถูกเปลี่ยนแปลงด้วยการเขียนโปรแกรม

เหตุการณ์ *OnChangs* จะไม่เกิดขึ้นถ้าเขตข้อมูลถูกเปลี่ยนแปลงโดยทางโปรแกรม *โดยใช้แอตทริบิวต์* [วิธี setValus](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ถ้าคุณต้องการให้ตัวจัดการเหตุการณ์เปิดให้เรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้เมธอด [fireOnchangy](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)ของแอตทริบิวต์ *formContext.data.entity* ในโค้ดของคุณ

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
