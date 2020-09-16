---
title: การแก้ไขปัญหาการรับรองความถูกต้องของ SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738008"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="1a63a-102">การแก้ไขปัญหาการรับรองความถูกต้องของ SMTP</span><span class="sxs-lookup"><span data-stu-id="1a63a-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="1a63a-103">ถ้าคุณได้รับข้อผิดพลาด5.7.57 หรือ5.7.3 เมื่อพยายามส่งอีเมล SMTP และการรับรองความถูกต้องด้วยไคลเอ็นต์หรือแอปพลิเคชันมีบางสิ่งที่คุณควรตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="1a63a-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="1a63a-104">การส่งการรับรองความถูกต้องของ SMTP อาจถูกปิดใช้งานในผู้เช่าของคุณหรือในกล่องจดหมายที่คุณกำลังพยายามใช้ (ตรวจสอบการตั้งค่าทั้งสองอย่าง)</span><span class="sxs-lookup"><span data-stu-id="1a63a-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="1a63a-105">เมื่อต้องการอ่านเพิ่มเติมให้ดูที่ [เปิดใช้งานหรือปิดใช้งานการส่ง SMTP ไคลเอ็นต์การรับรองความถูก](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)ต้อง</span><span class="sxs-lookup"><span data-stu-id="1a63a-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="1a63a-106">ตรวจสอบว่า [ค่าเริ่มต้นของความปลอดภัย Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ถูกเปิดใช้งานสำหรับผู้เช่าของคุณหรือไม่ ถ้าเปิดใช้งานการรับรองความถูกต้องของ SMTP โดยใช้การรับรองความถูกต้องเบื้องต้น (หรือที่เรียกว่าเก่าการทำเช่นนี้จะใช้ชื่อผู้ใช้และรหัสผ่าน) จะล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="1a63a-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
