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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714390"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="2d720-102">ไม่พบการสมัครใช้งานในศูนย์ความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="2d720-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="2d720-103">ถ้าในขณะที่เข้าถึงศูนย์การรักษาความปลอดภัยของ Microsoft Defender คุณได้รับข้อความ "ไม่มีการสมัครใช้งาน" หมายความว่า Azure Active Directory (AAD) ที่ใช้ในการเข้าสู่ระบบผู้ใช้พอร์ทัลไม่มีสิทธิ์การใช้งาน MICROSOFT Defender ATP</span><span class="sxs-lookup"><span data-stu-id="2d720-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="2d720-104">สิทธิ์การใช้งาน Windows E5 และ Office E5 เป็นสิทธิ์การใช้งานแยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="2d720-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="2d720-105">เปิดกรณีสนับสนุนถ้าซื้อสิทธิ์การใช้งานแต่ยังไม่ได้เตรียมใช้งานอินสแตนซ์ AAD นี้</span><span class="sxs-lookup"><span data-stu-id="2d720-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="2d720-106">คุณมี:</span><span class="sxs-lookup"><span data-stu-id="2d720-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="2d720-107">ปัญหาการเตรียมใช้งานสิทธิ์การใช้งานที่เป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="2d720-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="2d720-108">คุณเตรียมใช้งานสิทธิ์การใช้งาน Microsoft AAD อื่นโดยไม่ได้ตั้งใจซึ่งใช้การรับรองความถูกต้องในบริการ</span><span class="sxs-lookup"><span data-stu-id="2d720-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>