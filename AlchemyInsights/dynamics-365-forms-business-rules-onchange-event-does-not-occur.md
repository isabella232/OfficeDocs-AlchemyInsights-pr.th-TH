---
title: กฎทางธุรกิจ - กฎทางธุรกิจที่ไม่ได้ถูกใช้สำหรับแบบฟอร์มเป็นรูป Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529038"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>เหตุการณ์เกิดขึ้นถ้าเขตข้อมูลมีการเปลี่ยนแปลงโดยทางโปรแกรม

*เหตุการณ์*เกิดขึ้นถ้าเขตข้อมูลมีการเปลี่ยนแปลงโดยทางโปรแกรมโดยใช้การ*แอตทริบิวต์* วิธีการ[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ถ้าคุณต้องการให้ตัวจัดการเหตุการณ์สำหรับ*เหตุการณ์ที่จะเรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้*การ*แอตทริบิวต์ formContext.data.entity* วิธีการ[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)ในโค้ดของคุณ

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
