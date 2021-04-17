---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820197"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="a597d-102">การบล็อกการรับรองความถูกต้องแบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="a597d-102">Blocking legacy authentication</span></span>

<span data-ttu-id="a597d-103">การรับรองความถูกต้องแบบดั้งเดิมคือศัพท์ที่อ้างอิงถึงการร้องขอการรับรองความถูกต้องที่ถูกสร้างขึ้นโดย:</span><span class="sxs-lookup"><span data-stu-id="a597d-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="a597d-104">ไคลเอ็นต์ Office เวอร์ชันเก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบใหม่ (ตัวอย่างเช่น ไคลเอ็นต์ Office 2010)</span><span class="sxs-lookup"><span data-stu-id="a597d-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="a597d-105">ไคลเอ็นต์ใดๆ ที่ใช้โพรโทคอลจดหมายแบบดั้งเดิม เช่น IMAP/SMTP/POP3</span><span class="sxs-lookup"><span data-stu-id="a597d-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="a597d-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="a597d-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="a597d-107">ค่าเริ่มต้นด้านความปลอดภัยใน Azure Active Directory (Azure AD) ช่วยให้ง่ายต่อการรักษาความปลอดภัยและช่วยปกป้ององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="a597d-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="a597d-108">ค่าเริ่มต้นด้านความปลอดภัยประกอบด้วยการตั้งค่าความปลอดภัยที่ตั้งค่าไว้ล่วงหน้าของการโจมตีทั่วไป</span><span class="sxs-lookup"><span data-stu-id="a597d-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="a597d-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="a597d-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="a597d-110">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นในวันที่ 22 ตุลาคม 2019 หรือหลังจากวันที่ 22 ตุลาคม 2019 อาจเป็นไปได้ว่าคุณประสบกับลักษณะการรักษาความปลอดภัยตามค่าเริ่มต้นแบบใหม่ และมีการเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัยในผู้เช่าของคุณอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="a597d-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="a597d-111">ในความพยายามในการปกป้องผู้ใช้ของเราทั้งหมด ค่าเริ่มต้นด้านความปลอดภัยจะทยให้ผู้เช่าใหม่ทั้งหมดถูกสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="a597d-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
