---
title: สิทธิ์ API และกระบวนการให้ความยินยอม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405443"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="48ca9-102">สิทธิ์ API และกระบวนการให้ความยินยอม</span><span class="sxs-lookup"><span data-stu-id="48ca9-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="48ca9-103">เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม</span><span class="sxs-lookup"><span data-stu-id="48ca9-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="48ca9-104">[การอ้างอิงสิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="48ca9-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="48ca9-105">นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="48ca9-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="48ca9-106">**การตั้งค่าหรืออัปเดตหลักของบริการ**</span><span class="sxs-lookup"><span data-stu-id="48ca9-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="48ca9-107">[สร้าง serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - บทความนี้จะแสดงวิธีการสร้างวัตถุ servicePrincipal ใหม่</span><span class="sxs-lookup"><span data-stu-id="48ca9-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="48ca9-108">[สร้างบัญชีหลักของ& Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) ในพอร์ทัล - บทความนี้แสดงวิธีการสร้างแอปพลิเคชัน Azure Active Directory (Azure AD) ใหม่และหลักบริการที่สามารถใช้กับตัวควบคุมการเข้าถึงตามบทบาท</span><span class="sxs-lookup"><span data-stu-id="48ca9-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="48ca9-109">[แอป&](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) หลักบริการหลักใน Azure AD - บทความนี้อธิบายการลงทะเบียนแอปพลิเคชัน วัตถุแอปพลิเคชัน และหลักของบริการใน Azure Active Directory: สิ่งที่พวกเขาใช้ และวิธีการที่เกี่ยวข้องกัน</span><span class="sxs-lookup"><span data-stu-id="48ca9-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="48ca9-110">**เพิ่มหรืออัปเดตการลงทะเบียนแอปและให้ความยินยอมจากผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="48ca9-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="48ca9-111">[สร้างการลงทะเบียนแอป](https://docs.microsoft.com/graph/api/application-post-applications) - บทความนี้จะแสดงวิธีการสร้างวัตถุแอปพลิเคชันใหม่</span><span class="sxs-lookup"><span data-stu-id="48ca9-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="48ca9-112">[อัปเดตการลงทะเบียนแอป - สิทธิ์ API](https://docs.microsoft.com/graph/api/application-update) - บทความนี้จะแสดงวิธีการอัปเดตคุณสมบัติของวัตถุแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="48ca9-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="48ca9-113">[ให้ความยินยอมจาก](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) ผู้ดูแลระบบ - ในการยินยอมของผู้ดูแลระบบและความยินยอมทั่วไป เราต้องการให้ผู้ดูแลระบบอนุญาตการยินยอมอย่างชัดเจน</span><span class="sxs-lookup"><span data-stu-id="48ca9-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="48ca9-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - คอนเทนเนอร์การจัดการบทบาทเพื่อนิยามบทบาทที่เป็นหนึ่งเดียวและการมอบหมายบทบาทให้กับผู้ให้บริการ RBAC ของ Microsoft 365 ที่สนับสนุนหลักจํานวนมากและมีหลายขอบเขตในการมอบหมายบทบาทเดียว</span><span class="sxs-lookup"><span data-stu-id="48ca9-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="48ca9-115">ซึ่งแตกต่างจากชนิดทรัพยากร *rbacApplication*</span><span class="sxs-lookup"><span data-stu-id="48ca9-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="48ca9-116">Microsoft Intun1 เป็นตัวอย่างของผู้ให้บริการ RBAC ดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="48ca9-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="48ca9-117">การมอบหมายบทบาทใน Intun1 สามารถมีอาร์เรย์ของชื่อหลักและอาร์เรย์ของกลุ่มขอบเขตได้</span><span class="sxs-lookup"><span data-stu-id="48ca9-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="48ca9-118">**ค่านี้เป็นรุ่นเบต้า หมายความว่ายังอยู่ในช่วงการพัฒนาและไม่แนะนนะให้ใช้งานในการผลิต**</span><span class="sxs-lookup"><span data-stu-id="48ca9-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
