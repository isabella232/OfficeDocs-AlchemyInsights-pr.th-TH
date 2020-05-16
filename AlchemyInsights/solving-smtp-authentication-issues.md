---
title: การแก้ปัญหาการรับรองความถูกต้องของ SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264564"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="4fd21-102">การแก้ปัญหาการรับรองความถูกต้องของ SMTP</span><span class="sxs-lookup"><span data-stu-id="4fd21-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="4fd21-103">หากคุณได้รับข้อผิดพลาด 5.7.57 หรือ 5.7.3 เมื่อพยายามส่งอีเมล SMTP และรับรองความถูกต้องกับลูกค้าหรือโปรแกรมประยุกต์มีบางสิ่งที่คุณควรตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="4fd21-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="4fd21-104">การส่ง SMTP ที่รับรองความถูกต้องอาจถูกปิดใช้งานในผู้เช่าของคุณ หรือบนกล่องจดหมายที่คุณกําลังพยายามใช้ (ตรวจสอบการตั้งค่าทั้งสอง)</span><span class="sxs-lookup"><span data-stu-id="4fd21-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="4fd21-105">เมื่อต้องการอ่านเพิ่มเติม ให้ดูที่[การเปิดใช้งานหรือปิดใช้งานการส่ง SMTP ของไคลเอ็นต์ที่ได้รับการรับรองความถูกต้อง](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="4fd21-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="4fd21-106">ตรวจสอบว่า[ค่าเริ่มต้นการรักษาความปลอดภัย Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)จะเปิดใช้งานสําหรับผู้เช่าของคุณ ถ้าเปิดใช้งานการตรวจสอบสิทธิ์ SMTP โดยใช้การรับรองความถูกต้องพื้นฐาน (หรือที่เรียกว่าเดิม</span><span class="sxs-lookup"><span data-stu-id="4fd21-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
