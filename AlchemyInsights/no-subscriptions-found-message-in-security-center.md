---
title: ไม่พบการสมัครใช้งานในศูนย์ความปลอดภัย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544127"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="437ab-102">ไม่พบการสมัครใช้งานในศูนย์ความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="437ab-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="437ab-103">ถ้าขณะศูนย์การรักษาความปลอดภัยของ Microsoft Defenderเข้าถึง คุณจะได้รับข้อความ "ไม่มีการสมัครใช้งาน" หมายความว่า Azure Active Directory (AAD) ที่ใช้ในการเข้าสู่ระบบผู้ใช้ไปยังพอร์ทัลMicrosoft Defender ATPสิทธิ์การใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="437ab-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="437ab-104">The Windows E5 and Office E5 licenses are separate licenses.</span><span class="sxs-lookup"><span data-stu-id="437ab-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="437ab-105">เปิดกรณีการสนับสนุนถ้าซื้อสิทธิ์การใช้งานแต่ยังไม่ได้เตรียมใช้งานกับอินสแตนซ์ AAD นี้</span><span class="sxs-lookup"><span data-stu-id="437ab-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="437ab-106">คุณมีรายการใดรายการหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="437ab-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="437ab-107">ปัญหาการเตรียมใช้งานสิทธิ์การใช้งานที่เป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="437ab-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="437ab-108">คุณเตรียมใช้งานสิทธิ์การใช้งาน Microsoft AAD อื่นโดยไม่ได้ตั้งใจ ซึ่งใช้ในการรับรองความถูกต้องในบริการ</span><span class="sxs-lookup"><span data-stu-id="437ab-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>