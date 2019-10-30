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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769358"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="8763a-102">เหตุการณ์ OnChange ไม่เกิดขึ้นถ้าฟิลด์ถูกเปลี่ยนโดยทางโปรแกรม</span><span class="sxs-lookup"><span data-stu-id="8763a-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="8763a-103">เหตุการณ์*OnChange*ไม่เกิดขึ้นถ้าเขตข้อมูลถูกเปลี่ยนโดยทางโปรแกรมโดยใช้*แอตทริบิวต์* เมธอด[Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)</span><span class="sxs-lookup"><span data-stu-id="8763a-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="8763a-104">ถ้าคุณต้องการจัดการเหตุการณ์สำหรับเหตุการณ์*OnChange*ที่จะเรียกใช้หลังจากที่คุณตั้งค่าคุณต้องใช้*formcontext. ข้อมูลวิธี fireOnchange แอตทริบิวต์ของเอนทิตี* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)ในรหัสของคุณ</span><span class="sxs-lookup"><span data-stu-id="8763a-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
