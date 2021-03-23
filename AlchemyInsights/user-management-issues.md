---
title: ปัญหาการจัดการผู้ใช้
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037511"
---
# <a name="user-management-issues"></a><span data-ttu-id="3c292-102">ปัญหาการจัดการผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3c292-102">User management issues</span></span>

<span data-ttu-id="3c292-103">**What happens to current assigned users to the application if I disable the property 'User assignment required' (set this property to No)?**</span><span class="sxs-lookup"><span data-stu-id="3c292-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="3c292-104">การปิดใช้งาน **การมอบหมายของผู้ใช้** ที่ต้องใช้จะไม่มีผลต่อผู้ใช้ที่ได้รับมอบหมายในปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="3c292-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="3c292-105">การปิดใช้งานคุณสมบัตินี้จะอนุญาตให้ผู้ใช้ทั้งหมดเข้าถึงแอปพลิเคชันได้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="3c292-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="3c292-106">ผู้ใช้ที่แสดงอยู่ในรายการและผู้ใช้ที่ได้รับการมอบหมายให้กลุ่มในแอปพลิเคชันจะยังคงใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="3c292-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="3c292-107">เมื่อต้องการจํากัดแอปของคุณเฉพาะกลุ่มผู้ใช้ ให้ดู -[จํากัดแอป Azure AD เป็นชุดของผู้ใช้ - แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)</span><span class="sxs-lookup"><span data-stu-id="3c292-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="3c292-108">เมื่อต้องการกําหนดผู้ใช้และกลุ่ม ให้กับแอปพลิเคชันขององค์กรใน Azure Active Directory (Azure AD) จากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell ให้ดู จัดการงานที่มอบหมายของผู้ใช้ในแอป[ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)</span><span class="sxs-lookup"><span data-stu-id="3c292-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="3c292-109">เมื่อต้องการมอบสิทธิ์การสร้างและการจัดการแอปพลิเคชัน ให้ดู[มอบสิทธิ์ผู้ดูแลระบบแอปพลิเคชันในฐานะผู้รับมอบสิทธิ์ - Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)</span><span class="sxs-lookup"><span data-stu-id="3c292-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="3c292-110">**ซ่อนแอปองค์กรที่เฉพาะเจาะจงจากผู้ใช้**- ใช้ขั้นตอนต่อไปนี้เพื่อซ่อนแอป Microsoft 365 ทั้งหมดจาก **แผง MyApps**</span><span class="sxs-lookup"><span data-stu-id="3c292-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="3c292-111">แอปจะยังคงมองเห็นได้ในพอร์ทัล Office 365</span><span class="sxs-lookup"><span data-stu-id="3c292-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="3c292-112">ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบส่วนกลางของไดเรกทอรีของคุณ</span><span class="sxs-lookup"><span data-stu-id="3c292-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="3c292-113">เลือก **Azure Active Directory**</span><span class="sxs-lookup"><span data-stu-id="3c292-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="3c292-114">เลือก **ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="3c292-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="3c292-115">เลือก **การตั้งค่า** ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3c292-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="3c292-116">ภายใต้ **แอปพลิเคชัน** ขององค์กร ให้คลิก **จัดการวิธีเปิดใช้และดูแอปพลิเคชันของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="3c292-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="3c292-117">For **Users can only see Office 365 apps in the Office 365 portal,** click **Yes**.</span><span class="sxs-lookup"><span data-stu-id="3c292-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="3c292-118">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="3c292-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="3c292-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="3c292-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="3c292-120">ถ้าคุณเสนอแอปซอฟต์แวร์เป็นบริการ (SaaS) ให้กับองค์กรมากมาย คุณสามารถกําหนดค่าแอปให้ยอมรับการลงชื่อเข้าใช้จากผู้เช่า Azure Active Directory (Azure AD) ใดก็ได้</span><span class="sxs-lookup"><span data-stu-id="3c292-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="3c292-121">การกําหนดค่านี้เรียกว่า "การกําหนดให้แอปพลิเคชันของคุณมีหลายผู้เช่า"</span><span class="sxs-lookup"><span data-stu-id="3c292-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="3c292-122">ผู้ใช้ในผู้เช่า Azure AD จะสามารถลงชื่อเข้าใช้แอปของคุณหลังจากยินยอมให้ใช้บัญชีของพวกเขากับแอปของคุณ</span><span class="sxs-lookup"><span data-stu-id="3c292-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="3c292-123">For more information, see [build apps that sign in Azure AD users - Microsoft identity platform | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)</span><span class="sxs-lookup"><span data-stu-id="3c292-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="3c292-124">**ผู้ใช้ปลายทางจะสามารถเข้าถึงแอปพลิเคชันได้อย่างไรเมื่อเขา/เธอถูกมอบหมายไปยังแอปพลิเคชัน**</span><span class="sxs-lookup"><span data-stu-id="3c292-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="3c292-125">แต่ละแอปในใบแอปพลิเคชัน Enterprise จะมีลิงก์เพื่อให้ผู้ใช้เข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="3c292-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="3c292-126">ผู้ใช้ยังสามารถเข้าถึงแอปผ่าน **พอร์ทัลแอป** ของฉันด้วยวิธีง่ายๆ</span><span class="sxs-lookup"><span data-stu-id="3c292-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="3c292-127">**ต้องการทราบว่าผู้ใช้ใช้งานแอปพลิเคชันและแอปพลิเคชันชนิดใดอยู่หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="3c292-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="3c292-128">คุณสามารถดาวน์โหลดรายงานการลงชื่อเข้าใช้ในช่วง 30 วันที่ผ่านมาได้จาก **portal.azure.com > Azure Active Directory>ลงชื่อเข้าใช้>ดาวน์โหลดรายงาน**</span><span class="sxs-lookup"><span data-stu-id="3c292-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="3c292-129">เรียนรู้วิธีการให้ความยินยอม[จากผู้ดูแลระบบทั้งผู้เช่ากับแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)[และกําหนดว่าผู้ใช้จะยินยอมให้แอปพลิเคชันอนุญาตอย่างไร](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="3c292-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="3c292-130">เข้าใจ[วิธีการการยินยอม](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)[และจัดการความยินยอมใน](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)แอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="3c292-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


