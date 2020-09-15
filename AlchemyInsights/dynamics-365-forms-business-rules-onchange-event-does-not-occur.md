---
title: กฎทางธุรกิจของ Dynamics ๓๖๕แบบฟอร์ม-กฎทางธุรกิจไม่ยิงสำหรับฟอร์ม
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711510"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>เหตุการณ์ OnChange เกิดขึ้นถ้ามีการเปลี่ยนแปลงเขตข้อมูลโดยทางโปรแกรม

เหตุการณ์*OnChange*เกิดขึ้นถ้ามีการเปลี่ยนแปลงเขตข้อมูลโดยทางโปรแกรมโดยใช้*แอตทริบิวต์* วิธีที่[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ถ้าคุณต้องการให้ตัวจัดการเหตุการณ์สำหรับเหตุการณ์ *OnChange* ทำงานหลังจากที่คุณตั้งค่าคุณต้องใช้วิธีการ *formContext แอตทริบิวต์ของเอนทิตี* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) ในโค้ดของคุณ

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
