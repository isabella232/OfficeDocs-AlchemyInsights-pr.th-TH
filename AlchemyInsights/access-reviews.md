---
title: เข้าถึงรีวิว
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014995"
---
# <a name="access-reviews"></a><span data-ttu-id="e330d-102">เข้าถึงรีวิว</span><span class="sxs-lookup"><span data-stu-id="e330d-102">Access reviews</span></span>

1. <span data-ttu-id="e330d-103">**เปิดใช้งานรีวิวการเข้าถึง**: คุณสามารถเปิดใช้งานการรีวิวเมื่อคุณสร้างแพคเกจ access ใหม่หรือแก้ไขแพคเกจการเข้าถึงที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="e330d-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="e330d-104">[สร้างการตรวจทานการเข้าถึงของแพคเกจการเข้าถึงในการจัดการสิทธิ์ของ AZURE AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) อธิบายวิธีการเปิดใช้งานการเข้าถึงการเข้าถึงแพคเกจ access</span><span class="sxs-lookup"><span data-stu-id="e330d-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="e330d-105">**ตรวจทานการเข้าถึง**: การจัดการสิทธิ์การใช้งาน Azure AD ช่วยลดความซับซ้อนในการจัดการการเข้าถึงกลุ่มแอปพลิเคชันและไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="e330d-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="e330d-106">[ตรวจทานการเข้าถึงแพคเกจการเข้าถึงในการจัดการสิทธิ์การใช้งาน AZURE AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) อธิบายวิธีดำเนินการรีวิวการเข้าถึงสำหรับผู้ใช้อื่นที่ได้รับมอบหมายให้กับแพคเกจการเข้าถึงในฐานะผู้ตรวจทานที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="e330d-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="e330d-107">**ตรวจทานการเข้าถึงด้วยตัวคุณเอง**: การ [ตรวจสอบด้วยตนเองของแพคเกจการเข้าถึงในการจัดการสิทธิ์ของ AD Azure](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) อธิบายวิธีที่ผู้ใช้ตรวจทานตนเองของแพคเกจการเข้าถึงที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="e330d-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="e330d-108">ในกรณีส่วนใหญ่ผู้ใช้จะพบการรีวิวที่ค้างอยู่ในการตอบกลับของพวกเขาใน **แผงการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="e330d-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="e330d-109">การทำเช่นนี้จะสามารถใช้ได้กับความคิดเห็นของกลุ่มและแอปพลิเคชันไม่ใช่บทบาท</span><span class="sxs-lookup"><span data-stu-id="e330d-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="e330d-110">สำหรับความคิดเห็นของ Access ทั้งหมดของบทบาทผู้ใช้จะต้องนำทางไปยังการจัดการข้อมูลประจำตัวของ Azure AD AD (PIM) เพื่อทำการตรวจทานให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="e330d-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="e330d-111">การเข้าสู่ระบบไปยังพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="e330d-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="e330d-112">นำทางไปยัง Azure AD PIM</span><span class="sxs-lookup"><span data-stu-id="e330d-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="e330d-113">ในบานหน้าต่างนำทางด้านซ้ายให้เลือก **งาน**  >  การ **ตรวจทานการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="e330d-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="e330d-114">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="e330d-114">For more information, see:</span></span>

- [<span data-ttu-id="e330d-115">ดำเนินการรีวิว access ของบทบาท Azure AD Azure ของฉันใน PIM </span><span class="sxs-lookup"><span data-stu-id="e330d-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="e330d-116">ดำเนินการรีวิว access ของบทบาททรัพยากร Azure ของฉันใน PIM</span><span class="sxs-lookup"><span data-stu-id="e330d-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)