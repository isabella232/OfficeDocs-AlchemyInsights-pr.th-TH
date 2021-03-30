---
title: ปัญหาเจ้าของการลงทะเบียนแอป
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405323"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="1f7d5-102">ปัญหาเจ้าของการลงทะเบียนแอป</span><span class="sxs-lookup"><span data-stu-id="1f7d5-102">App Registration Owner issues</span></span>

<span data-ttu-id="1f7d5-103">ต่อไปนี้คือวิธีที่พร้อมใช้งานในการเพิ่มเงินต้นในฐานะเจ้าของในการลงทะเบียนแอป:</span><span class="sxs-lookup"><span data-stu-id="1f7d5-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="1f7d5-104">การใช้โมดูล Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="1f7d5-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="1f7d5-105">การอ้างอิง: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="1f7d5-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="1f7d5-106">การใช้ Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="1f7d5-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="1f7d5-107">การอ้างอิง: [เจ้าของแอป Az Ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="1f7d5-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="1f7d5-108">การใช้ MS Graph -</span><span class="sxs-lookup"><span data-stu-id="1f7d5-108">Using MS Graph -</span></span>

    <span data-ttu-id="1f7d5-109">การอ้างอิง: [เพิ่มเจ้าของ - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="1f7d5-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="1f7d5-110">การใช้พอร์ทัล Azure AD - นําทางไปยัง [portal.azure.com>](https://portal.azure.com/) Azure Active Directory >การลงทะเบียนแอป>เลือกแอปพลิเคชัน>เจ้าของ>เพิ่มเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="1f7d5-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="1f7d5-111">**ไม่สามารถดูแอปพลิเคชันของคุณบนใบลงทะเบียนแอปได้ แม้ว่าคุณจะเป็นเจ้าของแอปพลิเคชันนั้นหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="1f7d5-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="1f7d5-112">เจ้าของแอปไม่ใช่บทบาทการจัดการ</span><span class="sxs-lookup"><span data-stu-id="1f7d5-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="1f7d5-113">ถ้าการตั้งค่า [จํากัดการเข้าถึงพอร์ทัลการดูแลระบบ Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) ถูกเปิดใช้งาน เฉพาะผู้ดูแลระบบเท่านั้นที่สามารถดูแอปพลิเคชันบนพอร์ทัลการลงทะเบียนแอปได้</span><span class="sxs-lookup"><span data-stu-id="1f7d5-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="1f7d5-114">เพื่อให้เจ้าของสามารถดูแอปพลิเคชันได้ ให้ปิดใช้งานการตั้งค่านี้ (ตั้งค่านี้เป็น NO) หรือกําหนดบทบาทผู้ดูแลระบบให้เจ้าของเฉพาะแอปพลิเคชันที่ระบุเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="1f7d5-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="1f7d5-115">However for this, you will require an Azure AD Premium P2 license and [enable Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span><span class="sxs-lookup"><span data-stu-id="1f7d5-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
