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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748973"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="78477-102">เหตุการณ์เกิดขึ้นถ้าเขตข้อมูลมีการเปลี่ยนแปลงโดยทางโปรแกรม</span><span class="sxs-lookup"><span data-stu-id="78477-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="78477-103">*เหตุการณ์*เกิดขึ้นถ้าเขตข้อมูลมีการเปลี่ยนแปลงโดยทางโปรแกรมโดยใช้การ*แอตทริบิวต์* วิธีการ[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)</span><span class="sxs-lookup"><span data-stu-id="78477-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="78477-104">ถ้าคุณต้องการให้ตัวจัดการเหตุการณ์สำหรับ*เหตุการณ์ที่จะเรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้*การ*แอตทริบิวต์ formContext.data.entity* วิธีการ[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)ในโค้ดของคุณ</span><span class="sxs-lookup"><span data-stu-id="78477-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
