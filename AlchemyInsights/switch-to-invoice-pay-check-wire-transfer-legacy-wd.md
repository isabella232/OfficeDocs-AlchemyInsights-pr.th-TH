---
title: สลับไปยังใบแจ้งหนี้ชำระเงิน (เช็ค/โอนสาย)-แบบดั้งเดิม WD
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
- "9004168"
- "7343"
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/21/2020
ms.locfileid: "49726163"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="451b7-102">สลับไปยังใบแจ้งหนี้ชำระเงิน (เช็ค/โอนสาย)-แบบดั้งเดิม WD</span><span class="sxs-lookup"><span data-stu-id="451b7-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="451b7-103">ถ้าคุณสลับไปยังชำระเงินตามใบแจ้งหนี้นั่นหมายความว่าคุณจะชำระบิลของคุณภายใน30วันของวันที่ออกใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="451b7-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="451b7-104">เมื่อต้องการเข้าร่วมการชำระเงินสำหรับการสมัครใช้งาน Azure ของคุณโดยใช้ใบแจ้งหนี้ให้ส่งคำขอไปยังฝ่ายสนับสนุนของ Azure</span><span class="sxs-lookup"><span data-stu-id="451b7-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="451b7-105">เมื่อคำขอของคุณได้รับการอนุมัติคุณสามารถสลับการสมัครใช้งานการชำระเงินผ่านใบแจ้งหนี้ใน [พอร์ทัล Azure](https://portal.azure.com/)ได้</span><span class="sxs-lookup"><span data-stu-id="451b7-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="451b7-106">**ก่อนที่คุณจะดำเนินการต่อให้รีวิวข้อกำหนด/ข้อจำกัดต่อไปนี้ในการร้องขอตัวเลือกการชำระเงินตามใบแจ้งหนี้:**</span><span class="sxs-lookup"><span data-stu-id="451b7-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="451b7-107">ลงชื่อเข้าใช้ใน [พอร์ทัล Azure](https://portal.azure.com/) และนำทางไปยังวิธีการชำระเงิน</span><span class="sxs-lookup"><span data-stu-id="451b7-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="451b7-108">ตรวจสอบว่าคุณได้รับการอนุมัติการชำระเงินตามใบแจ้งหนี้ล่วงหน้าแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="451b7-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="451b7-109">การชำระเงินตามใบแจ้งหนี้จะพร้อมใช้งานสำหรับบัญชีธุรกิจเท่านั้นไม่ใช่สำหรับบัญชีส่วนบุคคล</span><span class="sxs-lookup"><span data-stu-id="451b7-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="451b7-110">คุณต้องชำระค่าใช้จ่ายค้างชำระทั้งหมดก่อนที่จะเปลี่ยนเป็นชำระเงินตามใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="451b7-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="451b7-111">ทีมสนับสนุนจะตรวจสอบบัญชีผู้ใช้เพื่อตรวจสอบว่ามีสิทธิ์สำหรับวิธีการชำระเงินตามใบแจ้งหนี้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="451b7-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="451b7-112">โหมดใบแจ้งหนี้ของการชำระเงินไม่ได้รับการสนับสนุนสำหรับบริการของบริษัทภายนอกของ marketplace ถ้าคุณต้องการสลับการสมัครใช้งานปัจจุบันไปยังใบแจ้งหนี้ที่มี marketplace หรือบริการของบริษัทอื่นบริการเหล่านี้จะต้องถูกลบก่อนที่จะสลับ</span><span class="sxs-lookup"><span data-stu-id="451b7-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="451b7-113">สำหรับบริการ marketplace ในอนาคตให้ซื้อการสมัครใช้งานแยกต่างหากบนบัตรเครดิตก่อนจากนั้นจึงซื้อหรือปรับใช้บริการของบริษัทที่สามของ marketplace</span><span class="sxs-lookup"><span data-stu-id="451b7-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="451b7-114">เมื่อคุณสลับไปยังใบแจ้งหนี้ชำระเงินแล้วคุณจะไม่สามารถสลับกลับไปที่การชำระเงินด้วยบัตรเครดิตหรือบัตรเดบิตได้</span><span class="sxs-lookup"><span data-stu-id="451b7-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="451b7-115">*เมื่อคุณได้รับอนุมัติการชำระเงินตามใบแจ้งหนี้* คุณสามารถสลับการสมัครใช้งาน Azure ของคุณไปยังใบแจ้งหนี้ชำระเงินผ่านทางเช็คหรือโอนสายใน  [พอร์ทัล Azure](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="451b7-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="451b7-116">เมื่อต้องการทำสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="451b7-116">To do that:</span></span>

1. <span data-ttu-id="451b7-117">ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://portal.azure.com/)ใน   ฐานะผู้ดูแลระบบบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="451b7-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="451b7-118">ค้นหาและเลือก **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="451b7-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="451b7-119">เลือกการสมัครใช้งานที่คุณต้องการสลับไปยังการชำระเงินตามใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="451b7-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="451b7-120">เลือก **วิธีการชำระเงิน**</span><span class="sxs-lookup"><span data-stu-id="451b7-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="451b7-121">ในแถบคำสั่งให้คลิกปุ่ม **ชำระเงินตามใบแจ้งหนี้**</span><span class="sxs-lookup"><span data-stu-id="451b7-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="451b7-122">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="451b7-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="451b7-123">ร้องขอ/ดาวน์โหลด/ดูใบแจ้งหนี้การเรียกเก็บเงินของ Azure และข้อมูลการใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="451b7-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="451b7-124">วิธีการส่งใบแจ้งหนี้ของ Azure ไปยังกล่องจดหมายเข้าของคุณโดยตรง</span><span class="sxs-lookup"><span data-stu-id="451b7-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="451b7-125">ชำระเงินตามใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="451b7-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="451b7-126">ทำความเข้าใจเกี่ยวกับค่าใช้จ่ายในการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="451b7-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="451b7-127">ทำความเข้าใจเกี่ยวกับข้อกำหนดในใบแจ้งหนี้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="451b7-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="451b7-128">วิธีการโอนความเป็นเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="451b7-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
