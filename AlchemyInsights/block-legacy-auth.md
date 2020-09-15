---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685617"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="cd055-102">การบล็อกการรับรองความถูกต้องแบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="cd055-102">Blocking legacy authentication</span></span>

<span data-ttu-id="cd055-103">การรับรองความถูกต้องแบบดั้งเดิมคือคำที่อ้างอิงถึงคำขอการรับรองความถูกต้องที่ทำโดย:</span><span class="sxs-lookup"><span data-stu-id="cd055-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="cd055-104">ไคลเอ็นต์ Office รุ่นเก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบสมัยใหม่ (ตัวอย่างเช่นไคลเอ็นต์ Office ๒๐๑๐)</span><span class="sxs-lookup"><span data-stu-id="cd055-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="cd055-105">ไคลเอ็นต์ใดๆที่ใช้โพรโทคอลของจดหมายแบบดั้งเดิมเช่น IMAP/SMTP/POP3</span><span class="sxs-lookup"><span data-stu-id="cd055-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="cd055-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการบล็อกการรับรองความถูกต้องแบบดั้งเดิมและการเปิดใช้งานการรับรองความถูกต้องแบบใหม่ให้ดูที่การ[บล็อกการรับรอง](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="cd055-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="cd055-107">ค่าเริ่มต้นของความปลอดภัยใน Azure Active Directory (Azure AD) ทำให้ง่ายต่อการรักษาความปลอดภัยและช่วยปกป้ององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="cd055-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="cd055-108">ค่าเริ่มต้นของความปลอดภัยมีการตั้งค่าความปลอดภัยที่กำหนดไว้ล่วงหน้าสำหรับการโจมตีทั่วไป</span><span class="sxs-lookup"><span data-stu-id="cd055-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="cd055-109">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับค่าเริ่มต้นด้านความปลอดภัยให้ดูที่[ค่าเริ่มต้นด้านความปลอดภัยคืออะไร](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="cd055-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="cd055-110">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหรือหลังจากวันที่22ตุลาคม๒๐๑๙อาจเป็นไปได้ว่าคุณกำลังประสบกับลักษณะการทำงานที่มีการรักษาความปลอดภัยใหม่และมีค่าเริ่มต้นของความปลอดภัยที่เปิดใช้งานในผู้เช่าของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="cd055-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="cd055-111">ในความพยายามที่จะปกป้องผู้ใช้ทั้งหมดของเราค่าเริ่มต้นการรักษาความปลอดภัยจะถูกยกเลิกไปยังผู้เช่าใหม่ทั้งหมดที่สร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="cd055-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
