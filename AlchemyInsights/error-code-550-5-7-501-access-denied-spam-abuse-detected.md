---
title: รหัสข้อผิดพลาด 550 5.7.501 ปฏิเสธการตรวจพบการละเมิดสแปม
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 7be23f02878d12aa08cb4970af6f99539a9cefab
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703045"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="4ba9b-102">550 5.7.501 ปฏิเสธการเข้าถึง, สแปมการละเมิดตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="4ba9b-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="4ba9b-103">โดยทั่วไป ข้อความนี้เกิดขึ้นเมื่อผู้ใช้ส่งข้อความอีเมล์จากที่อยู่ IP โดยใช้โดเมน*เริ่มต้น.onmicrosoft.com*ที่กําหนดให้กับผู้เช่าใหม่ใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4ba9b-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="4ba9b-104">วิธีที่ง่ายที่สุดในการแก้ไขปัญหานี้คือ:</span><span class="sxs-lookup"><span data-stu-id="4ba9b-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="4ba9b-105">[เพิ่มโดเมนในผู้เช่าของคุณ](https://docs.microsoft.com//office365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="4ba9b-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="4ba9b-106">[เปลี่ยนที่อยู่อีเมลหลักของผู้ใช้](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address)เป็นโดเมนแบบกําหนดเองใหม่ที่คุณเพิ่งเพิ่ม</span><span class="sxs-lookup"><span data-stu-id="4ba9b-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
