---
title: รหัสข้อผิดพลาด๕๕๐5.7.501 การเข้าถึงถูกปฏิเสธตรวจพบการละเมิดสแปม
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36740160"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="356a2-102">๕๕๐5.7.501 เข้าถึงถูกปฏิเสธการละเมิดสแปมที่ตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="356a2-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="356a2-103">ข้อความนี้จะเกิดขึ้นเมื่อผู้ใช้ส่งข้อความทางเมลจากที่อยู่ IP โดยใช้โดเมน*onmicrosoft.com*เริ่มต้นที่ถูกกำหนดให้กับผู้เช่าใหม่ใน Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="356a2-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="356a2-104">วิธีที่ง่ายที่สุดในการแก้ไขปัญหานี้คือ:</span><span class="sxs-lookup"><span data-stu-id="356a2-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="356a2-105">[เพิ่มโดเมนในผู้เช่าของคุณ](https://docs.microsoft.com//office365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="356a2-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="356a2-106">[เปลี่ยนที่อยู่เมลหลักของผู้ใช้ของคุณ](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address)เป็นโดเมนที่กำหนดเองใหม่ที่คุณเพิ่งเพิ่มเข้ามา</span><span class="sxs-lookup"><span data-stu-id="356a2-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
