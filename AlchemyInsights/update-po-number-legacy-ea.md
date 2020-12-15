---
title: อัปเดตหมายเลข PO-ขั้นตอนที่แนะนำ EA
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/09/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9004166"
- "7322"
ms.openlocfilehash: ef1e5f52cb26542892199694309fb2b0df551997
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679595"
---
# <a name="update-purchase-order-number---legacy-ea---recommended-steps"></a><span data-ttu-id="9a886-102">อัปเดตหมายเลขใบสั่งซื้อ-ขั้นตอนที่แนะนำของ EA แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="9a886-102">Update Purchase Order number - Legacy EA - recommended steps</span></span>

<span data-ttu-id="9a886-103">การเปลี่ยนแปลงหมายเลขใบสั่งซื้อ (PO) จะมีผลกับใบแจ้งหนี้ถัดไป</span><span class="sxs-lookup"><span data-stu-id="9a886-103">Changes to the purchase order (PO) number will take effect on the next invoice.</span></span> <span data-ttu-id="9a886-104">เมื่อต้องการเปลี่ยนหมายเลข PO บนใบแจ้งหนี้ที่สร้างขึ้นแล้วให้เปิดบัตรสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="9a886-104">To change the PO number on an invoice that has already been generated, open a support ticket.</span></span> 

<span data-ttu-id="9a886-105">พอร์ทัล EA ของ Azure จะสร้างหมายเลข PO เริ่มต้นโดยอัตโนมัติยกเว้นว่าผู้ดูแลระบบ EA ตั้งค่าก่อนวันที่ในใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="9a886-105">The Azure EA portal automatically generates a default PO number unless the EA admin sets one before the invoice date.</span></span> <span data-ttu-id="9a886-106">ในฐานะผู้ดูแลระบบ EA (การลงทะเบียนโดยตรง)/ผู้ดูแลระบบคู่ค้า (การลงทะเบียนทางอ้อม) คุณสามารถอัปเดตหมายเลข PO ในพอร์ทัล EA ของ Azure ได้</span><span class="sxs-lookup"><span data-stu-id="9a886-106">As an EA Administrator (Direct Enrollment) / Partner Administrator (Indirect Enrollment), you can update the PO number in the Azure EA portal.</span></span> <span data-ttu-id="9a886-107">เมื่อต้องการอัปเดตหมายเลข PO:</span><span class="sxs-lookup"><span data-stu-id="9a886-107">To update the PO number:</span></span>

1. <span data-ttu-id="9a886-108">ลงชื่อเข้าใช้พอร์ทัล EA</span><span class="sxs-lookup"><span data-stu-id="9a886-108">Sign into EA portal.</span></span>
2. <span data-ttu-id="9a886-109">คลิก **รายงาน** ทางด้านซ้ายมือ</span><span class="sxs-lookup"><span data-stu-id="9a886-109">Click **Reports** on the left-hand side.</span></span>
3. <span data-ttu-id="9a886-110">คลิก **สรุปการใช้งาน** ที่ด้านบนของหน้า</span><span class="sxs-lookup"><span data-stu-id="9a886-110">Click **Usage Summary** at the top of the page.</span></span>
4. <span data-ttu-id="9a886-111">เลือกช่วงเวลาที่เกี่ยวข้องจากรายการดรอปดาวน์</span><span class="sxs-lookup"><span data-stu-id="9a886-111">Select the relevant period from the drop-down list.</span></span>
5. <span data-ttu-id="9a886-112">คลิก **ดู/แก้ไขหมายเลข PO**</span><span class="sxs-lookup"><span data-stu-id="9a886-112">Click **View/Edit PO Numbers**.</span></span>
6. <span data-ttu-id="9a886-113">ใส่หมายเลข PO ใหม่แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="9a886-113">Enter the new PO number and click **Save**.</span></span>

<span data-ttu-id="9a886-114">คุณสามารถอัพเดตหมายเลข PO ได้ตลอดเวลาก่อนที่จะมีการสร้างใบแจ้งหนี้สำหรับช่วงเวลาการเรียกเก็บเงินปัจจุบันและไม่เกิน7วันหลังจากที่ได้รับอีเมลแจ้งให้ทราบเกี่ยวกับใบแจ้งหนี้อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="9a886-114">You can update the PO number at any time prior to the invoice being generated for the current billing period, and up to seven days after receiving the automated invoice notification email.</span></span> 

<span data-ttu-id="9a886-115">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="9a886-115">**Recommended documents**</span></span>

- [<span data-ttu-id="9a886-116">ใบแจ้งหนี้การลงทะเบียนขององค์กร Azure</span><span class="sxs-lookup"><span data-stu-id="9a886-116">Azure enterprise enrollment invoices</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-enrollment-invoices) 
- [<span data-ttu-id="9a886-117">ทำความเข้าใจใบเรียกเก็บเงินข้อตกลงองค์กร Azure ของคุณ</span><span class="sxs-lookup"><span data-stu-id="9a886-117">Understand your Azure Enterprise Agreement bill</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/review-enterprise-agreement-bill)  
- [<span data-ttu-id="9a886-118">ทำความเข้าใจเกี่ยวกับบทบาทขององค์กร Azure</span><span class="sxs-lookup"><span data-stu-id="9a886-118">Understand Azure Enterprise roles</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-ea-roles#add-a-new-enterprise-administrator) 
- [<span data-ttu-id="9a886-119">สร้างผู้ดูแลระบบขององค์กรอื่น (ผู้ดูแลระบบ EA)</span><span class="sxs-lookup"><span data-stu-id="9a886-119">Create another enterprise administrator (EA Admin)</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-administration#create-another-enterprise-administrator)
