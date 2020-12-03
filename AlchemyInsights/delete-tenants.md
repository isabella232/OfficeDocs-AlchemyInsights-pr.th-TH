---
title: ลบผู้เช่า
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564878"
---
# <a name="delete-tenant"></a><span data-ttu-id="36f94-102">ลบผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="36f94-102">Delete tenant</span></span>

<span data-ttu-id="36f94-103">เมื่อต้องการลบโฆษณา Azure ให้ตรวจสอบให้แน่ใจว่า:</span><span class="sxs-lookup"><span data-stu-id="36f94-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="36f94-104">คุณเป็นผู้ดูแลระบบส่วนกลางบนไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="36f94-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="36f94-105">คุณไม่ได้ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีไดเรกทอรีเริ่มต้นเช่น contoso.onmicrosoft.com ในบัญชีผู้ใช้ที่ลงชื่อเข้าใช้เช่น admin@contoso.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="36f94-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="36f94-106">เอาแอปพลิเคชันที่ใช้งานอยู่ในไดเรกทอรีออกก่อนการลบ</span><span class="sxs-lookup"><span data-stu-id="36f94-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="36f94-107">เมื่อต้องการเอาแอปพลิเคชันที่ใช้งานอยู่ออกให้นำทางไปยังการลงทะเบียนแอปและเอาแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="36f94-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="36f94-108">ไม่มีการสมัครใช้งานที่ใช้งานอยู่สำหรับบริการ Microsoft Online ใดๆเช่น Microsoft Azure, Office ๓๖๕หรือ Azure AD Premium ที่เกี่ยวข้องกับไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="36f94-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="36f94-109">โอนการสมัครใช้งานของคุณหรือยกเลิกการสมัครใช้งานที่ใช้งานได้ผ่านทางการสนับสนุนและการเรียกเก็บเงินของ Azure</span><span class="sxs-lookup"><span data-stu-id="36f94-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="36f94-110">เรียนรู้เพิ่มเติมเกี่ยวกับวิธีการยกเลิกการสมัครใช้งาน Office ๓๖๕และ Azure</span><span class="sxs-lookup"><span data-stu-id="36f94-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="36f94-111">สำหรับคำแนะนำเกี่ยวกับการเชื่อมโยงหรือการเพิ่มการสมัครใช้งานที่มีอยู่ให้กับผู้เช่าให้ดูที่[เชื่อมโยงหรือเพิ่มการสมัครใช้งาน azure ไปยังผู้เช่า AZURE AD ของคุณ](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)</span><span class="sxs-lookup"><span data-stu-id="36f94-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="36f94-112">ไม่มีสิทธิ์การใช้งานที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="36f94-112">There are no Active license.</span></span> <span data-ttu-id="36f94-113">เมื่อต้องการเอาสิทธิ์การใช้งานออกให้ดู[วิธีการเอาการสมัครใช้งานออกเพื่อเอาสิทธิ์การใช้งานออก](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)</span><span class="sxs-lookup"><span data-stu-id="36f94-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="36f94-114">ไม่มีผู้ใช้ที่ใช้งานอยู่อื่นในไดเรกทอรีนอกเหนือจากตัวคุณเองเป็นผู้ดูแลระบบส่วนกลางเมื่อพยายามลบโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="36f94-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="36f94-115">เอาผู้ใช้ที่ใช้งานอยู่และการอ้างอิงใดๆบนชื่อโดเมนแบบกำหนดเองในผู้เช่าจะต้องถูกเอาออกเช่นผู้ใช้ที่สร้างด้วย admin@contoso.com</span><span class="sxs-lookup"><span data-stu-id="36f94-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="36f94-116">สำหรับขั้นตอนรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการ:</span><span class="sxs-lookup"><span data-stu-id="36f94-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="36f94-117">ลบ "Azure Active Directory" หรือ "การสมัครใช้งาน" ให้ดู[ลบไดเรกทอรีที่ใช้งานอยู่ของ azure](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)</span><span class="sxs-lookup"><span data-stu-id="36f94-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="36f94-118">การเอาแอปพลิเคชันในไดเรกทอรีออกให้ดูที่การ [เอาแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)ออก</span><span class="sxs-lookup"><span data-stu-id="36f94-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
