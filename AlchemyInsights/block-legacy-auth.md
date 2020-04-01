---
title: บล็อกดั้งเดิม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079279"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="83995-102">การบล็อกการรับรองความถูกต้องแบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="83995-102">Blocking legacy authentication</span></span>

<span data-ttu-id="83995-103">การรับรองความถูกต้องแบบดั้งเดิมเป็นคําที่อ้างถึงการร้องขอการรับรองความถูกต้องที่ทําโดย:</span><span class="sxs-lookup"><span data-stu-id="83995-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="83995-104">ไคลเอ็นต์ Office เก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบสมัยใหม่ (ตัวอย่างเช่น ไคลเอ็นต์ Office 2010)</span><span class="sxs-lookup"><span data-stu-id="83995-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="83995-105">ไคลเอ็นต์ใด ๆ ที่ใช้โพรโทคอลจดหมายแบบดั้งเดิมเช่น IMAP/SMTP/POP3</span><span class="sxs-lookup"><span data-stu-id="83995-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="83995-106">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการบล็อกการรับรองความถูกต้องแบบดั้งเดิมและเปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่ ให้ดูที่[การบล็อกการรับรองความถูกต้องแบบดั้งเดิม](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="83995-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="83995-107">ค่าเริ่มต้นการรักษาความปลอดภัยใน Azure Active Directory (Azure AD) ช่วยให้มีความปลอดภัยและช่วยปกป้ององค์กรของคุณได้ง่ายขึ้น</span><span class="sxs-lookup"><span data-stu-id="83995-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="83995-108">ค่าเริ่มต้นความปลอดภัยมีการตั้งค่าความปลอดภัยที่กําหนดไว้ล่วงหน้าสําหรับการโจมตีทั่วไป</span><span class="sxs-lookup"><span data-stu-id="83995-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="83995-109">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับค่าเริ่มต้นความปลอดภัย ให้ดูที่[ค่าเริ่มต้นความปลอดภัยคืออะไร](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="83995-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="83995-110">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นในวันที่ หรือหลังวันที่ 22 ตุลาคม 2019 เป็นไปได้ว่าคุณประสบกับลักษณะการทํางานที่ปลอดภัยโดยเริ่มต้นใหม่ และได้เปิดใช้ค่าเริ่มต้นการรักษาความปลอดภัยในผู้เช่าของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="83995-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="83995-111">ในความพยายามที่จะปกป้องผู้ใช้ทั้งหมดของเราค่าเริ่มต้นการรักษาความปลอดภัยจะถูกรีดออกไปยังผู้เช่าใหม่ทั้งหมดที่สร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="83995-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
