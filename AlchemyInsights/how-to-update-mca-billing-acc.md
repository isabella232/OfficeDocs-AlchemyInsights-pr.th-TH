---
title: อัปเดตที่อยู่ขายและเรียกเก็บเงินที่เชื่อมโยงกับขั้นตอนที่แนะนำ MCA ของคุณ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679979"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="8d81a-102">อัปเดตที่อยู่ขายและเรียกเก็บเงินที่เชื่อมโยงกับขั้นตอนที่แนะนำ MCA ของคุณ</span><span class="sxs-lookup"><span data-stu-id="8d81a-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="8d81a-103">คุณสามารถอัพเดตที่อยู่ขายและเรียกเก็บเงินที่เกี่ยวข้องกับข้อตกลงลูกค้าของ Microsoft (MCA) ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="8d81a-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="8d81a-104">เฉพาะผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถทำการเปลี่ยนแปลงกับข้อมูลโปรไฟล์ผู้ใช้ Active Directory ของ Azure ได้</span><span class="sxs-lookup"><span data-stu-id="8d81a-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="8d81a-105">ถ้าคุณไม่ได้กำหนดบทบาทผู้ดูแลระบบของผู้ใช้ให้ติดต่อผู้ดูแลระบบผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="8d81a-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="8d81a-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนโปรไฟล์ของผู้ใช้ให้ดูที่[เพิ่มหรืออัปเดตข้อมูลโปรไฟล์ของผู้ใช้โดยใช้ Azure Active directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="8d81a-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="8d81a-107">**ที่อยู่ที่ขาย** แล้ว-ที่อยู่ที่ขายเป็นที่อยู่และข้อมูลที่ติดต่อขององค์กรหรือบุคคลที่รับผิดชอบสำหรับบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="8d81a-108">ซึ่งจะแสดงในใบแจ้งหนี้ทั้งหมดที่สร้างขึ้นสำหรับบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="8d81a-109">**ที่อยู่สำหรับเรียกเก็บเงิน** -ที่อยู่เรียกเก็บเงินคือที่อยู่และข้อมูลที่ติดต่อขององค์กรหรือบุคคลที่รับผิดชอบสำหรับใบแจ้งหนี้ที่สร้างขึ้นสำหรับบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="8d81a-110">สำหรับบัญชีการเรียกเก็บเงินสำหรับ MCA มีที่อยู่เรียกเก็บเงินสำหรับโปรไฟล์การเรียกเก็บเงินแต่ละรายการและแสดงอยู่ในใบแจ้งหนี้ที่สร้างขึ้นสำหรับโปรไฟล์การเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="8d81a-111">**เมื่อต้องการอัปเดตบัญชีผู้ใช้สำหรับการเรียกเก็บเงินแบบ MCA ที่อยู่ที่จำหน่าย**:</span><span class="sxs-lookup"><span data-stu-id="8d81a-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="8d81a-112">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้ที่อยู่อีเมลที่มีเจ้าของหรือบทบาทผู้สนับสนุนในบัญชีการเรียกเก็บเงินสำหรับ MCA</span><span class="sxs-lookup"><span data-stu-id="8d81a-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="8d81a-113">ค้นหาการ  +  **เรียกเก็บเงิน** การจัดการต้นทุน</span><span class="sxs-lookup"><span data-stu-id="8d81a-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="8d81a-114">คลิก **คุณสมบัติ** การ  >  **อัปเดตที่ขายไปยัง**</span><span class="sxs-lookup"><span data-stu-id="8d81a-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="8d81a-115">ใส่ที่อยู่ใหม่แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="8d81a-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="8d81a-116">บัญชีบางบัญชีจำเป็นต้องมีการตรวจสอบเพิ่มเติมก่อนที่จะสามารถอัปเดตที่อยู่ที่ขายไปยังที่อยู่</span><span class="sxs-lookup"><span data-stu-id="8d81a-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="8d81a-117">ถ้าบัญชีผู้ใช้ของคุณจำเป็นต้องมีการอนุมัติด้วยตนเองคุณจะถูกขอให้ติดต่อฝ่ายสนับสนุนของ Azure</span><span class="sxs-lookup"><span data-stu-id="8d81a-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="8d81a-118">**เมื่อต้องการอัปเดตที่อยู่บัญชีการเรียกเก็บเงินของ MCA**:</span><span class="sxs-lookup"><span data-stu-id="8d81a-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="8d81a-119">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้ที่อยู่อีเมลที่มีเจ้าของหรือบทบาทผู้สนับสนุนในบัญชีการเรียกเก็บเงินหรือโปรไฟล์การเรียกเก็บเงินสำหรับ MCA</span><span class="sxs-lookup"><span data-stu-id="8d81a-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="8d81a-120">ค้นหาการ  +  **เรียกเก็บเงิน** การจัดการต้นทุน</span><span class="sxs-lookup"><span data-stu-id="8d81a-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="8d81a-121">คลิก **โปรไฟล์การเรียกเก็บเงิน** และเลือกโปรไฟล์การเรียกเก็บเงินเพื่ออัปเดตที่อยู่สำหรับเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="8d81a-122">คลิก **คุณสมบัติ**  >  การ **อัปเดตที่อยู่**</span><span class="sxs-lookup"><span data-stu-id="8d81a-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="8d81a-123">ใส่ที่อยู่ใหม่แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="8d81a-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="8d81a-124">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="8d81a-124">**Recommended documents**</span></span>

<span data-ttu-id="8d81a-125">[เปลี่ยนข้อมูลที่ติดต่อสำหรับบัญชีผู้ใช้การเรียกเก็บเงิน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="8d81a-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="8d81a-126">อัปเดตการตั้งค่าบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="8d81a-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="8d81a-127">ทำความเข้าใจเกี่ยวกับบทบาทการดูแลข้อตกลงของลูกค้าของ Microsoft ใน Azure</span><span class="sxs-lookup"><span data-stu-id="8d81a-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)