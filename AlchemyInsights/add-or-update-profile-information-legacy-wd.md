---
title: เพิ่มหรืออัปเดตข้อมูลโปรไฟล์-ขั้นตอนที่แนะนำ WD-แบบดั้งเดิม
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/10/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9004166"
- "7339"
ms.openlocfilehash: a3cbf78949c7e22d537f54c2498133277a6cb5d6
ms.sourcegitcommit: 830aeb6797075d79e3a3006da05da2059ddd041f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679850"
---
# <a name="add-or-update-profile-information---legacy-wd---recommended-steps"></a><span data-ttu-id="ed9fe-102">เพิ่มหรืออัปเดตข้อมูลโปรไฟล์-ขั้นตอนที่แนะนำ WD-แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="ed9fe-102">Add or update profile information - Legacy WD - recommended steps</span></span>

<span data-ttu-id="ed9fe-103">**เปลี่ยนข้อมูลที่ติดต่อสำหรับบัญชีผู้ใช้การเรียกเก็บเงิน Azure**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-103">**Change contact information for an Azure billing account**</span></span>

<span data-ttu-id="ed9fe-104">**ที่อยู่เรียกเก็บเงิน**: ที่อยู่เรียกเก็บเงินคือที่อยู่และข้อมูลที่ติดต่อขององค์กรหรือบุคคลที่รับผิดชอบการชำระเงินสำหรับใบแจ้งหนี้ที่สร้างขึ้นสำหรับบัญชีการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="ed9fe-104">**Bill-to address**: The bill-to address is the address and the contact information of the organization or the individual, who is responsible for payment for the invoices generated for a billing account.</span></span> <span data-ttu-id="ed9fe-105">สำหรับ [บัญชีการเรียกเก็บเงินสำหรับโปรแกรม Microsoft Online Service (MOSP)](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#update-an-mosp-billing-account-address)จะมีที่อยู่เรียกเก็บเงินหนึ่งรายการซึ่งจะแสดงอยู่บนใบแจ้งหนี้ทั้งหมดที่สร้างขึ้นสำหรับลูกค้าองค์กร</span><span class="sxs-lookup"><span data-stu-id="ed9fe-105">For a [billing account for a Microsoft Online Service Program (MOSP)](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#update-an-mosp-billing-account-address), there's one bill-to address, which is displayed on all the invoices generated for the account.</span></span>

<span data-ttu-id="ed9fe-106">**ที่อยู่อีเมลที่ติดต่อสำหรับบริการและอีเมลสำหรับการตลาด**: คุณสามารถ [ระบุที่อยู่อีเมลที่](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#change-your-contact-email-address) แตกต่างจากที่อยู่อีเมลที่คุณลงชื่อเข้าใช้เพื่อรับการแจ้งเตือนที่เกี่ยวข้องกับการเรียกเก็บเงินที่เกี่ยวข้องกับบริการและคำแนะนำเกี่ยวกับการแจ้งเตือนเกี่ยวกับบัญชีผู้ใช้ Azure ของคุณ</span><span class="sxs-lookup"><span data-stu-id="ed9fe-106">**Contact email address for service and marketing emails**: You can [specify an email address](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#change-your-contact-email-address) that's different from the email address that you sign in with to receive important billing-related, service-related, and recommendation-related notifications about your Azure account.</span></span> <span data-ttu-id="ed9fe-107">อีเมลการแจ้งเตือนบริการเช่นปัญหาด้านความปลอดภัยด่วนการเปลี่ยนแปลงราคาหรือการแบ่งการเปลี่ยนแปลงที่เกิดขึ้นกับบริการที่ใช้โดยบัญชีผู้ใช้ของคุณจะถูกส่งไปยังที่อยู่การลงชื่อเข้าใช้ของคุณเสมอ</span><span class="sxs-lookup"><span data-stu-id="ed9fe-107">Service notification emails, such as urgent security issues, price changes, or breaking changes to services in use by your account, are always sent to your sign-in address.</span></span>

<span data-ttu-id="ed9fe-108">เมื่อต้องการอัปเดตที่อยู่ของบัญชีผู้ใช้การเรียกเก็บเงิน MOSP ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ed9fe-108">To update an MOSP billing account address, complete the following steps:</span></span>
1. <span data-ttu-id="ed9fe-109">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้ที่อยู่อีเมลที่มีสิทธิ์ผู้ดูแลระบบบัญชีผู้ใช้ในบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="ed9fe-109">Sign in to the Azure portal using the email address which has the account administrator permission on the account.</span></span>
2. <span data-ttu-id="ed9fe-110">ค้นหาและเลือก **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-110">Search for and select **Cost Management + Billing**.</span></span> 
3. <span data-ttu-id="ed9fe-111">คลิก **คุณสมบัติ** จากด้านซ้ายมือ</span><span class="sxs-lookup"><span data-stu-id="ed9fe-111">Click **Properties** from the left-hand side.</span></span> 
4. <span data-ttu-id="ed9fe-112">คลิก **อัปเดตที่อยู่สำหรับการเรียกเก็บเงิน** เพื่ออัปเดตที่อยู่และที่อยู่เรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="ed9fe-112">Click **Update billing address** to update the sold-to and the bill-to addresses.</span></span> <span data-ttu-id="ed9fe-113">ใส่ที่อยู่ใหม่แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-113">Enter the new address, and then click **Save**.</span></span>

<span data-ttu-id="ed9fe-114">**เปลี่ยนที่อยู่อีเมลของที่ติดต่อของคุณ**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-114">**Change your contact email address**</span></span> 

<span data-ttu-id="ed9fe-115">เมื่อต้องการเปลี่ยนที่อยู่อีเมลของที่ติดต่อของคุณให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ed9fe-115">To change your contact email address, complete the following steps:</span></span>
1. <span data-ttu-id="ed9fe-116">ถ้าคุณเป็นผู้ดูแลระบบบัญชีผู้ใช้สำหรับบัญชีผู้ใช้ MOSP ให้ทำตามคำแนะนำใน [อัปเดตที่อยู่บัญชีผู้ใช้การเรียกเก็บเงิน MOSP](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#update-an-mosp-billing-account-address) แล้วคลิก **อัปเดตข้อมูลที่ติดต่อ** ในขั้นตอนสุดท้าย</span><span class="sxs-lookup"><span data-stu-id="ed9fe-116">If you're an account administrator for an MOSP account, follow the instructions in [Update an MOSP billing account address](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile#update-an-mosp-billing-account-address) and click **Update contact info** in the last step.</span></span> 
2. <span data-ttu-id="ed9fe-117">ใส่ที่อยู่อีเมลใหม่</span><span class="sxs-lookup"><span data-stu-id="ed9fe-117">Enter the new email address.</span></span> 
3. <span data-ttu-id="ed9fe-118">ไปที่บานหน้าต่าง [ข้อมูลที่ติดต่อ](https://ms.portal.azure.com/) ในพอร์ทัล Azure แล้วใส่ที่อยู่อีเมลใหม่</span><span class="sxs-lookup"><span data-stu-id="ed9fe-118">Go to the [Contact information](https://ms.portal.azure.com/) pane in the Azure portal and enter the new email address.</span></span> 
4. <span data-ttu-id="ed9fe-119">คลิกที่ไอคอนที่มีชื่อย่อหรือรูปภาพของคุณ</span><span class="sxs-lookup"><span data-stu-id="ed9fe-119">Click the icon with your initials or picture.</span></span> 
5. <span data-ttu-id="ed9fe-120">เลือก **เมนูบริบท (...) > ข้อมูลที่ติดต่อของฉัน** แล้วใส่ที่อยู่อีเมลใหม่</span><span class="sxs-lookup"><span data-stu-id="ed9fe-120">Select **context menu (...) > My Contact Information**, and enter the new email address.</span></span>

<span data-ttu-id="ed9fe-121">**เพิ่มหรืออัปเดตข้อมูลโปรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-121">**Add or update profile information**</span></span>

<span data-ttu-id="ed9fe-122">คุณสามารถเพิ่มข้อมูลส่วนกำหนดค่าผู้ใช้รวมถึงรูปภาพโปรไฟล์ข้อมูลเฉพาะของงานและการตั้งค่าบางอย่างโดยใช้ Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ed9fe-122">You can add user profile information, including a profile picture, job-specific information, and some settings, using Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ed9fe-123">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเพิ่มผู้ใช้ใหม่ให้ดู[ที่วิธีการเพิ่มหรือลบผู้ใช้ใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)</span><span class="sxs-lookup"><span data-stu-id="ed9fe-123">For more information about adding new users, see [How to add or delete users in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).</span></span>

<span data-ttu-id="ed9fe-124">เมื่อต้องการเพิ่มหรือเปลี่ยนข้อมูลโปรไฟล์ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ed9fe-124">To add or change profile information, complete the following steps:</span></span>

1. <span data-ttu-id="ed9fe-125">ลงชื่อเข้าใช้พอร์ทัล Azure เป็นผู้ใช้-ผู้ดูแลระบบสำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="ed9fe-125">Sign in to the Azure portal as a user-administrator for the organization.</span></span>
2. <span data-ttu-id="ed9fe-126">เลือก **ผู้ใช้ Azure Active directory >** จากนั้นคลิกโปรไฟล์ผู้ใช้ที่คุณต้องการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="ed9fe-126">Select **Azure Active Directory > Users**, and then click the user profile you'd like to update.</span></span> 
3. <span data-ttu-id="ed9fe-127">คลิก **แก้ไข** เพื่อเลือกเพิ่มหรืออัปเดตข้อมูลที่รวมอยู่ในส่วนที่พร้อมใช้งานแต่ละส่วน</span><span class="sxs-lookup"><span data-stu-id="ed9fe-127">Click **Edit** to optionally add or update the information included in each of the available sections.</span></span> 
4. <span data-ttu-id="ed9fe-128">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-128">Click **Save**.</span></span>

<span data-ttu-id="ed9fe-129">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="ed9fe-129">**Recommended documents**</span></span>

- [<span data-ttu-id="ed9fe-130">บัญชีผู้ใช้และขอบเขตการเรียกเก็บเงินในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="ed9fe-130">Billing accounts and scopes in the Azure portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/view-all-accounts) 
- [<span data-ttu-id="ed9fe-131">เพิ่มหรืออัปเดตข้อมูลบัตรเครดิตสำหรับ Azure</span><span class="sxs-lookup"><span data-stu-id="ed9fe-131">Add or update a credit card for Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)


