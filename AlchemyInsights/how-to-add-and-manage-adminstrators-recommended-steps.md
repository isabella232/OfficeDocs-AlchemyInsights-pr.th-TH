---
title: วิธีการเพิ่มและจัดการ adminstrators-ขั้นตอนที่แนะนำ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678869"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="3f7b1-102">วิธีการเพิ่มและจัดการ adminstrators-ขั้นตอนที่แนะนำ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="3f7b1-103">**แก้ไขผู้ดูแลระบบการสมัครใช้งานหรือผู้ดูแลระบบร่วม**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="3f7b1-104">ผู้ดูแลระบบบัญชีผู้ใช้สามารถแก้ไขทั้งสองบทบาทได้ในขณะที่ผู้ดูแลระบบการสมัครใช้งานสามารถเปลี่ยนได้เฉพาะผู้ดูแลร่วมใน [พอร์ทัล Azure](https://ms.portal.azure.com/#home)เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="3f7b1-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="3f7b1-105">เพิ่มหรือเปลี่ยนแปลงผู้ดูแลการสมัครใช้งาน Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="3f7b1-106">**อัปเดตผู้ดูแลการสมัครใช้งานหรือการสมัครใช้งาน Co-Administrator สำหรับการสมัครใช้งานภายใน (ออก)**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="3f7b1-107">ผู้ดูแลระบบบริการหรือผู้ดูแลร่วมสามารถใช้งานการกระทำนี้ได้โดยใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3f7b1-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="3f7b1-108">ลงชื่อเข้าใช้ใน [พอร์ทัล Azure](https://ms.portal.azure.com/#home) แล้วคลิก **การจัดการต้นทุน + การเรียกเก็บเงิน** ในใบมีดซ้าย</span><span class="sxs-lookup"><span data-stu-id="3f7b1-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="3f7b1-109">คลิกบรรทัดรายการที่มีการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="3f7b1-110">ซึ่งจะเป็นการเปิดภาพรวมสำหรับการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="3f7b1-111">บนใบมีดการ **สมัคร** ใช้งานให้คลิก **คุณสมบัติ**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="3f7b1-112">คลิกปุ่ม **ผู้ดูแลระบบบริการ**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="3f7b1-113">ใส่อีเมลของผู้ใช้ที่คุณต้องการตั้งค่าเป็นผู้ดูแลระบบบริการแล้วคลิก **ตกลง**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="3f7b1-114">**เพิ่ม/เปลี่ยน/เอาผู้ดูแลร่วมออก**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="3f7b1-115">ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://ms.portal.azure.com/#home) ในฐานะผู้ดูแลระบบบริการ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="3f7b1-116">เปิดการ [สมัคร](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ใช้งานแล้วเลือกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="3f7b1-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="3f7b1-117">(Adminstrators สามารถกำหนดได้เฉพาะในขอบเขตการสมัครใช้งานเท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="3f7b1-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="3f7b1-118">นำทางไปยังผู้ดูแลการ **เข้าถึงตัวควบคุม (IAM)**  >  **Classic**  >  **เพิ่ม**  >  **เพิ่มผู้ดูแล** เมื่อต้องการเปิดบานหน้าต่าง **เพิ่มการจัดการร่วม**(ถ้ามีการปิดใช้งานตัวเลือกเพิ่มการดูแลระบบ) แสดงว่าคุณไม่มีสิทธิ์)</span><span class="sxs-lookup"><span data-stu-id="3f7b1-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="3f7b1-119">เลือกผู้ใช้ที่คุณต้องการเพิ่มแล้วคลิก **เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="3f7b1-120">**ศึกษาเพิ่มเติม:**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-120">**Learn more:**</span></span>
- [<span data-ttu-id="3f7b1-121">เพิ่มผู้ดูแลร่วม</span><span class="sxs-lookup"><span data-stu-id="3f7b1-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3f7b1-122">เอาผู้ดูแลร่วมออก</span><span class="sxs-lookup"><span data-stu-id="3f7b1-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3f7b1-123">เปลี่ยนผู้ดูแลระบบบริการ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3f7b1-124">ดูผู้ดูแลระบบบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3f7b1-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3f7b1-125">จัดการการเข้าถึงโดยใช้ RBAC และพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="3f7b1-126">**เพิ่ม/ลบผู้ใช้ที่ใช้ Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="3f7b1-127">คุณสามารถเพิ่มผู้ใช้ใหม่หรือลบผู้ใช้ที่มีอยู่ออกจากองค์กร Azure Active Directory (Azure AD) ของคุณได้ดังนี้</span><span class="sxs-lookup"><span data-stu-id="3f7b1-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="3f7b1-128">เมื่อต้องการเพิ่มผู้ใช้ใหม่ให้เข้าสู่ระบบ [พอร์ทัล Azure](https://ms.portal.azure.com/#home) เป็นผู้ดูแลระบบผู้ใช้สำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="3f7b1-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="3f7b1-129">เลือก **Azure Active directory** เลือก **ผู้ใช้** แล้วคลิก **ผู้ใช้ใหม่**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="3f7b1-130">บนหน้า **ผู้ใช้** ให้กรอกข้อมูลที่จำเป็น</span><span class="sxs-lookup"><span data-stu-id="3f7b1-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="3f7b1-131">คลิก **สร้าง**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-131">Click **Create**.</span></span> <span data-ttu-id="3f7b1-132">ผู้ใช้จะถูกสร้างขึ้นและเพิ่มลงในผู้เช่า Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3f7b1-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="3f7b1-133">**เรียนรู้เพิ่มเติม**:</span><span class="sxs-lookup"><span data-stu-id="3f7b1-133">**Learn more**:</span></span>

- [<span data-ttu-id="3f7b1-134">เพิ่มผู้ใช้ใหม่</span><span class="sxs-lookup"><span data-stu-id="3f7b1-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3f7b1-135">ลบผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3f7b1-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3f7b1-136">เพิ่มหรืออัปเดตข้อมูลโปรไฟล์ของผู้ใช้โดยใช้ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3f7b1-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="3f7b1-137">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="3f7b1-137">**Recommended documents**</span></span>

- [<span data-ttu-id="3f7b1-138">การควบคุมการเข้าถึงตามบทบาท (RBAC) คืออะไร</span><span class="sxs-lookup"><span data-stu-id="3f7b1-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="3f7b1-139">ทำความเข้าใจบทบาทที่แตกต่างกันใน Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="3f7b1-140">สิทธิ์ของบทบาทผู้ดูแลระบบใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3f7b1-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="3f7b1-141">บทช่วยสอน: ให้สิทธิ์การเข้าถึงสำหรับผู้ใช้ที่ใช้ RBAC และพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="3f7b1-142">แก้ไขปัญหา RBAC ใน Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="3f7b1-143">จัดระเบียบทรัพยากรของคุณด้วยกลุ่มการจัดการ Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="3f7b1-144">วิธีการร้องขอสำเนาใบแจ้งหนี้ของ Azure ผ่านทางอีเมล</span><span class="sxs-lookup"><span data-stu-id="3f7b1-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="3f7b1-145">วิธีการเพิ่มอัปเดตหรือเอาบัตรเครดิตหรือบัตรเดบิตออกจาก Azure</span><span class="sxs-lookup"><span data-stu-id="3f7b1-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="3f7b1-146">การสมัครใช้งาน (เปิดใช้งาน/ยกเลิก/สลับ)</span><span class="sxs-lookup"><span data-stu-id="3f7b1-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



