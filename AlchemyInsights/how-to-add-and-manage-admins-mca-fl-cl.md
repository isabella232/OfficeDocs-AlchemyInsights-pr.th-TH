---
title: วิธีการเพิ่มและจัดการผู้ดูแลระบบ-ชั้น MCA/CL
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692315"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="f2c1b-102">วิธีการเพิ่มและจัดการผู้ดูแลระบบ-ชั้น MCA/CL</span><span class="sxs-lookup"><span data-stu-id="f2c1b-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="f2c1b-103">เมื่อต้องการจัดการบัญชีผู้ใช้สำหรับการเรียกเก็บเงินของคุณสำหรับข้อตกลงลูกค้าของ Microsoft (MCA) คุณสามารถใช้บทบาทที่แตกต่างกันกับระดับการเข้าถึงที่ต้องการได้</span><span class="sxs-lookup"><span data-stu-id="f2c1b-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="f2c1b-104">บทบาทเหล่านี้นอกเหนือจากบทบาทบริการ Azure ที่มีอยู่แล้วภายในซึ่งจะช่วยให้คุณสามารถควบคุมทรัพยากรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="f2c1b-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="f2c1b-105">**เมื่อต้องการเพิ่มบทบาทการเรียกเก็บเงินในพอร์ทัล Azure ให้ใช้ดังนี้**</span><span class="sxs-lookup"><span data-stu-id="f2c1b-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="f2c1b-106">ลงชื่อเข้าใช้[พอร์ทัล Azure](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="f2c1b-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f2c1b-107">ค้นหา *การจัดการต้นทุน + การเรียกเก็บเงิน*</span><span class="sxs-lookup"><span data-stu-id="f2c1b-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="f2c1b-108">เลือกตัวควบคุมการเข้าถึง (IAM) ที่ขอบเขตเช่นบัญชีผู้ใช้การเรียกเก็บเงินโปรไฟล์การเรียกเก็บเงินหรือใบแจ้งหนี้ที่คุณต้องการให้สิทธิ์การเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="f2c1b-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="f2c1b-109">หน้า Access control (IAM) จะแสดงรายการผู้ใช้และกลุ่มที่ได้รับมอบหมายให้กับแต่ละบทบาทสำหรับขอบเขตนั้น</span><span class="sxs-lookup"><span data-stu-id="f2c1b-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="f2c1b-110">เมื่อต้องการให้สิทธิ์การเข้าถึงแก่ผู้ใช้ให้เลือก **เพิ่ม** จากด้านบนของหน้า</span><span class="sxs-lookup"><span data-stu-id="f2c1b-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="f2c1b-111">ในรายการดรอปดาวน์ *บทบาท* ให้เลือกบทบาท</span><span class="sxs-lookup"><span data-stu-id="f2c1b-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="f2c1b-112">ใส่ที่อยู่อีเมลของผู้ใช้ที่คุณต้องการให้สิทธิ์การเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="f2c1b-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="f2c1b-113">เลือก **บันทึก** เพื่อกำหนดบทบาท</span><span class="sxs-lookup"><span data-stu-id="f2c1b-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="f2c1b-114">เมื่อต้องการเอา access ออกจากผู้ใช้ให้เลือกผู้ใช้ที่มีการกำหนดบทบาทที่คุณต้องการเอาออก</span><span class="sxs-lookup"><span data-stu-id="f2c1b-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="f2c1b-115">เลือก **นำออก**</span><span class="sxs-lookup"><span data-stu-id="f2c1b-115">Select **Remove**.</span></span>

<span data-ttu-id="f2c1b-116">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="f2c1b-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="f2c1b-117">ข้อกำหนดบทบาทของการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="f2c1b-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="f2c1b-118">บทบาทและงานของบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="f2c1b-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="f2c1b-119">เริ่มต้นใช้งานบัญชีการเรียกเก็บเงิน MCA ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2c1b-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="f2c1b-120">ตรวจสอบการเข้าถึงข้อตกลงลูกค้าของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="f2c1b-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
