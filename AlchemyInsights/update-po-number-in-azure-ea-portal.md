---
title: อัปเดตหมายเลข PO ใน Azure EA portal-ขั้นตอนที่แนะนำ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/17/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7290"
ms.openlocfilehash: 0388ffa5e33cca366ab02c93bb70464fb2453752
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714953"
---
# <a name="update-po-number-in-azure-ea-portal---recommended-steps"></a><span data-ttu-id="5cebf-102">อัปเดตหมายเลข PO ใน Azure EA portal-ขั้นตอนที่แนะนำ</span><span class="sxs-lookup"><span data-stu-id="5cebf-102">Update PO number in Azure EA portal - recommended steps</span></span>

<span data-ttu-id="5cebf-103">การเปลี่ยนแปลงหมายเลขบัญชี VAT/ภาษีหรือใบสั่งซื้อ (PO) จะมีผลกับใบแจ้งหนี้ถัดไป</span><span class="sxs-lookup"><span data-stu-id="5cebf-103">Changes to the VAT/TAX ID or purchase order (PO) number will take effect on the next invoice.</span></span> <span data-ttu-id="5cebf-104">เมื่อต้องการเปลี่ยน ID ของ VAT/ภาษีหรือหมายเลข PO เป็นใบแจ้งหนี้ที่สร้างขึ้นแล้วให้เปิดบัตรสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="5cebf-104">To change the VAT/TAX ID or PO number to an invoice that has already been generated, open a support ticket.</span></span> <span data-ttu-id="5cebf-105">ถ้าคุณมีปัญหาใดๆที่เกี่ยวข้องกับ ID VAT/ภาษีของคุณให้ติดต่อกับคู่ค้าของ Microsoft Licensing (คู่ค้าหรือที่ปรึกษาซอฟต์แวร์)</span><span class="sxs-lookup"><span data-stu-id="5cebf-105">If you have any issues related to your VAT/TAX ID, reach out to your Microsoft Licensing Partner (Partner or a Software Advisor).</span></span> <span data-ttu-id="5cebf-106">พวกเขาจะติดต่อศูนย์การดำเนินการภูมิภาค (ROC) สำหรับคำถามเกี่ยวกับ ID VAT/ภาษีของคุณ</span><span class="sxs-lookup"><span data-stu-id="5cebf-106">They'll contact the Regional Operations Center (ROC) for questions regarding your VAT/TAX ID.</span></span> 

<span data-ttu-id="5cebf-107">พอร์ทัล EA ของ Azure จะสร้างหมายเลข PO เริ่มต้นโดยอัตโนมัติยกเว้นว่าผู้ดูแลระบบ EA ตั้งค่าก่อนวันที่ในใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="5cebf-107">The Azure EA portal automatically generates a default  PO number unless the EA admin sets one before the invoice date.</span></span> <span data-ttu-id="5cebf-108">ในฐานะผู้ดูแลระบบ EA (การลงทะเบียนโดยตรง)/ผู้ดูแลระบบคู่ค้า (การลงทะเบียนทางอ้อม) คุณสามารถอัปเดตหมายเลข PO ในพอร์ทัล EA ของ Azure ได้</span><span class="sxs-lookup"><span data-stu-id="5cebf-108">As an EA Administrator (Direct Enrollment) / Partner Administrator (Indirect Enrollment), you can update the PO number in the Azure EA portal.</span></span> <span data-ttu-id="5cebf-109">คุณสามารถอัพเดตหมายเลข PO ได้ตลอดเวลาก่อนที่จะมีการสร้างใบแจ้งหนี้สำหรับระยะเวลาการเรียกเก็บเงินปัจจุบันและไม่เกินเจ็ดวันหลังจากได้รับอีเมลแจ้งเตือนเกี่ยวกับใบแจ้งหนี้อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5cebf-109">You can update the PO number at any time prior to the invoice being generated for the current billing period and up to seven days after receiving the automated invoice notification email.</span></span>    

<span data-ttu-id="5cebf-110">เมื่อต้องการอัปเดตหมายเลข PO:</span><span class="sxs-lookup"><span data-stu-id="5cebf-110">To update the PO number:</span></span>

1. <span data-ttu-id="5cebf-111">ลงชื่อเข้าใช้[พอร์ทัล EA](https://ea.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="5cebf-111">Sign into [EA portal](https://ea.azure.com/).</span></span>
1. <span data-ttu-id="5cebf-112">ในบานหน้าต่างด้านซ้ายให้คลิก **รายงาน**</span><span class="sxs-lookup"><span data-stu-id="5cebf-112">In the left pane, click **Reports**.</span></span>
1. <span data-ttu-id="5cebf-113">ที่ด้านบนของหน้าให้คลิก **สรุปการใช้งาน** แล้วเลือกระยะเวลาที่เกี่ยวข้องจากเมนูดรอปดาวน์</span><span class="sxs-lookup"><span data-stu-id="5cebf-113">At the top of the page, click **Usage Summary** and select the select the relevant period from the dropdown.</span></span>
1. <span data-ttu-id="5cebf-114">คลิก **ดู/แก้ไขหมายเลข PO**</span><span class="sxs-lookup"><span data-stu-id="5cebf-114">Click **View/Edit PO Numbers**.</span></span>
1. <span data-ttu-id="5cebf-115">ใส่หมายเลข PO ใหม่แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="5cebf-115">Enter the new PO number and click **Save**.</span></span>

<span data-ttu-id="5cebf-116">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="5cebf-116">**Recommended documents**</span></span> 

- [<span data-ttu-id="5cebf-117">ใบแจ้งหนี้การลงทะเบียนขององค์กร Azure</span><span class="sxs-lookup"><span data-stu-id="5cebf-117">Azure enterprise enrollment invoices</span></span>](https://docs.microsoft.com/azure/billing/billing-ea-portal-enrollment-invoices) 
- [<span data-ttu-id="5cebf-118">ทำความเข้าใจใบเรียกเก็บเงินข้อตกลงองค์กร Azure ของคุณ</span><span class="sxs-lookup"><span data-stu-id="5cebf-118">Understand your Azure Enterprise Agreement bill</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill-ea)  
- [<span data-ttu-id="5cebf-119">ทำความเข้าใจเกี่ยวกับบทบาทขององค์กร Azure</span><span class="sxs-lookup"><span data-stu-id="5cebf-119">Understand Azure Enterprise roles</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill-ea) 
- [<span data-ttu-id="5cebf-120">สร้างผู้ดูแลระบบขององค์กรอื่น (ผู้ดูแลระบบ EA)</span><span class="sxs-lookup"><span data-stu-id="5cebf-120">Create another enterprise administrator (EA Admin)</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-administration#create-another-enterprise-administrator) 
