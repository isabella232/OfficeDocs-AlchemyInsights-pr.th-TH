---
title: ปัญหาเกี่ยวกับการอ้างสิทธิ์และแอตทริบิวต์โทเค็น
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036078"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="09d0b-102">ปัญหาเกี่ยวกับการอ้างสิทธิ์และแอตทริบิวต์โทเค็น</span><span class="sxs-lookup"><span data-stu-id="09d0b-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="09d0b-103">**อัปเดต กําหนดค่า หรือเอาการอ้างสิทธิ์โทเค็นออก**</span><span class="sxs-lookup"><span data-stu-id="09d0b-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="09d0b-104">ด้วยการใช้ Azure Active Directory (Azure AD) คุณสามารถปรับแต่งชนิดการอ้างสิทธิ์ของ [บทบาทใน](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) โทเค็นตอบกลับที่คุณได้รับหลังจากที่คุณอนุญาตแอปได้</span><span class="sxs-lookup"><span data-stu-id="09d0b-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="09d0b-105">นักพัฒนาแอปพลิเคชันสามารถใช้การอ้างสิทธิ์เพิ่มเติมในแอปพลิเคชัน Azure AD เพื่อระบุการอ้างสิทธิ์ที่พวกเขาต้องการในโทเค็นที่ส่งไปยังแอปพลิเคชันของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="09d0b-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="09d0b-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="09d0b-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="09d0b-107">[กําหนดค่าการอ้างสิทธิ์กลุ่มของแอปพลิเคชันด้วย Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="09d0b-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="09d0b-108">ถ้าใช้การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่นในแอปพลิเคชันของคุณ ให้ดู[การอ้างสิทธิ์แบบปรับแต่งที่ออกในโทเค็น SAML ของแอปพลิเคชันขององค์กร](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="09d0b-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="09d0b-109">**การอ้างสิทธิ์การแมปแอตทริบิวต์**</span><span class="sxs-lookup"><span data-stu-id="09d0b-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="09d0b-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="09d0b-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="09d0b-111">แอตทริบิวต์ส่วนขยาย Schema ไดเรกทอรีมีวิธีการจัดเก็บข้อมูลเพิ่มเติมใน Azure Active Directory บนวัตถุผู้ใช้และวัตถุไดเรกทอรีอื่นๆ เช่น กลุ่ม รายละเอียดผู้เช่า หลักบริการ</span><span class="sxs-lookup"><span data-stu-id="09d0b-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="09d0b-112">เฉพาะแอตทริบิวต์ส่วนขยายบนวัตถุของผู้ใช้เท่านั้นที่สามารถใช้ในการอ้างสิทธิ์ไปยังแอปพลิเคชันได้</span><span class="sxs-lookup"><span data-stu-id="09d0b-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="09d0b-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span><span class="sxs-lookup"><span data-stu-id="09d0b-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="09d0b-114">ดูข้อมูลเพิ่มเติมเกี่ยวกับการอ้างสิทธิ์โทเค็นที่:</span><span class="sxs-lookup"><span data-stu-id="09d0b-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="09d0b-115">อ้างสิทธิ์ในโทเค็นการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="09d0b-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="09d0b-116">การอ้างสิทธิ์ในid_token</span><span class="sxs-lookup"><span data-stu-id="09d0b-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="09d0b-117">[การอ้าง](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) สิทธิ์ที่คุณสามารถคาดหวังในโทเค็น ID และโทเค็นการเข้าถึงที่ออกโดย Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="09d0b-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="09d0b-118">การอ้างอิงการอ้างสิทธิ์โทเค็น SAML</span><span class="sxs-lookup"><span data-stu-id="09d0b-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
