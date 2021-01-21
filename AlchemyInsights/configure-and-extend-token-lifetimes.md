---
title: กำหนดค่าและขยายระยะเวลาของโทเค็น
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917197"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="ada1c-102">กำหนดค่าและขยายระยะเวลาของโทเค็น</span><span class="sxs-lookup"><span data-stu-id="ada1c-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="ada1c-103">คุณสามารถระบุอายุการใช้งานของโทเค็นการเข้าถึง SAML หรือ ID ที่ออกโดย Microsoft identity platform</span><span class="sxs-lookup"><span data-stu-id="ada1c-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="ada1c-104">คุณสามารถตั้งค่าการหมดอายุของโทเค็นสำหรับแอปทั้งหมดในองค์กรของคุณสำหรับแอปพลิเคชันแบบหลายผู้เช่า (หลายองค์กร) หรือสำหรับบริการหลักที่เฉพาะเจาะจงในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ada1c-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="ada1c-105">สำหรับข้อมูลเพิ่มเติมให้อ่านช่วงเวลาของ [โทเค็น](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)ที่กำหนดค่าไว้</span><span class="sxs-lookup"><span data-stu-id="ada1c-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="ada1c-106">ตัวอย่างเช่นอ่าน[ตัวอย่างของวิธีการกำหนดค่าการหมดอายุของโทเค็น](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="ada1c-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="ada1c-107">เมื่อต้องการเรียนรู้วิธีการกำหนดค่าอายุการใช้งานและความเข้ากันได้ของโทเค็นใน Azure Active Directory B2C (Azure AD B2C) ให้ดู [ที่การกำหนดค่าโทเค็นใน B2C Azure active](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)directory</span><span class="sxs-lookup"><span data-stu-id="ada1c-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="ada1c-108">บทความการ [กำหนดค่าลักษณะการทำงานของเซสชันใน B2C Azure active](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) directory จะอธิบายวิธีการลงชื่อเข้าระบบครั้งเดียว (SSO) ที่ใช้ใน B2C AD Azure และช่วยให้คุณเลือกวิธีที่เหมาะสมที่สุดของ SSO เมื่อกำหนดค่านโยบายของคุณ</span><span class="sxs-lookup"><span data-stu-id="ada1c-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="ada1c-109">**โทเค็นจะมีระยะเวลานานแค่ไหน พวกเขาจะใช้งานได้นานแค่ไหน**</span><span class="sxs-lookup"><span data-stu-id="ada1c-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="ada1c-110">อายุการใช้งานของโทเค็นคือ1ชั่วโมงและอายุการใช้งานของเซสชันคือ24ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="ada1c-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="ada1c-111">ซึ่งหมายความว่าถ้าไม่มีการร้องขอใน24ชั่วโมงคุณจำเป็นต้องเข้าสู่ระบบอีกครั้งก่อนที่จะร้องขอโทเค็นใหม่</span><span class="sxs-lookup"><span data-stu-id="ada1c-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="ada1c-112">หลังจาก30พฤษภาคม๒๐๒๐ไม่มีผู้เช่าใหม่จะสามารถใช้นโยบายอายุการใช้งานโทเค็นที่กำหนดค่าเพื่อกำหนดค่าเซสชันและการรีเฟรชโทเค็น</span><span class="sxs-lookup"><span data-stu-id="ada1c-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="ada1c-113">แผนจะเกิดขึ้นภายในหลายเดือนหลังจากนั้นซึ่งหมายความว่าเราจะหยุดการ honoring เซสชันที่มีอยู่และการรีเฟรช</span><span class="sxs-lookup"><span data-stu-id="ada1c-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="ada1c-114">คุณยังสามารถกำหนดค่าความหมดอายุของโทเค็นการเข้าถึงหลังจากแผนได้</span><span class="sxs-lookup"><span data-stu-id="ada1c-114">You can still configure access token lifetimes after the deprecation.</span></span>






