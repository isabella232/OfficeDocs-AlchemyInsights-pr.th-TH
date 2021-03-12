---
title: ปัญหาเกี่ยวกับผู้เช่า
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714483"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="65b15-102">ปัญหาเกี่ยวกับผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="65b15-102">Issues with tenants</span></span>

<span data-ttu-id="65b15-103">Azure Active Directory (Azure AD) จะจัดระเบียบวัตถุ เช่น ผู้ใช้และแอปให้เป็นกลุ่มที่เรียกว่าผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="65b15-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="65b15-104">ผู้เช่าอนุญาตให้ผู้ดูแลระบบตั้งค่านโยบายเกี่ยวกับผู้ใช้ภายในองค์กรและแอปที่องค์กรเป็นเจ้าของเป็นไปตามนโยบายความปลอดภัยและการปฏิบัติการของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="65b15-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="65b15-105">For more information, see [tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span><span class="sxs-lookup"><span data-stu-id="65b15-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="65b15-106">For more information related to tenant management, see the following articles:</span><span class="sxs-lookup"><span data-stu-id="65b15-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="65b15-107">[การเริ่มต้นใช้งานด่วน: ตั้งค่าผู้เช่า](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - แสดงวิธีการสร้างผู้เช่าใหม่</span><span class="sxs-lookup"><span data-stu-id="65b15-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="65b15-108">[ลบผู้เช่าใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - แสดงวิธีการลบผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="65b15-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="65b15-109">**ปัญหาเกี่ยวกับหลายผู้เช่า**</span><span class="sxs-lookup"><span data-stu-id="65b15-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="65b15-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span><span class="sxs-lookup"><span data-stu-id="65b15-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="65b15-111">[วิธีการ: ลงชื่อเข้าใช้ผู้ใช้ Azure Active Directory ใดๆ โดยใช้](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) รูปแบบแอปพลิเคชันหลายผู้เช่า - แสดงวิธีการแปลงจากผู้เช่าเดียวเป็นแอปพลิเคชันหลายผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="65b15-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="65b15-112">[ตั้งค่าการลงชื่อเข้าใช้](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) ขององค์กร Azure Active Directory ใน Azure Active Directory B2C - แสดงวิธีการเปิดใช้งานการลงชื่อเข้าใช้ของผู้ใช้จากองค์กร Azure AD ที่ระบุโดยใช้โฟลว์ผู้ใช้ใน Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="65b15-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="65b15-113">[ตั้งค่าการลงชื่อเข้าใช้](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  แบบหลายผู้เช่า Azure Active Directory โดยใช้นโยบายแบบปรับแต่งเองใน Azure Active Directory B2C แสดงวิธีการเปิดใช้งานการลงชื่อเข้าใช้ของผู้ใช้ที่ใช้จุดสิ้นสุดแบบหลายผู้เช่าของ Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="65b15-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






