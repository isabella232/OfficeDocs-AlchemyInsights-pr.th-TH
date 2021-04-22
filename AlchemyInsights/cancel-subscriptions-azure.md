---
title: ยกเลิกการสมัครใช้งานใน Azure
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003797"
- "6786"
ms.openlocfilehash: 83fab49ccafd23352fe28569289a709a198fd402
ms.sourcegitcommit: 80a36e6447953b3f65e45c05607dbfc585fbf8b0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2021
ms.locfileid: "51936173"
---
# <a name="cancel-subscription"></a><span data-ttu-id="d50a8-102">ยกเลิกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="d50a8-102">Cancel Subscription</span></span>

<span data-ttu-id="d50a8-103">ถ้าคุณไม่ต้องการการสมัครใช้งาน Azure อีกต่อไป คุณสามารถยกเลิกการสมัครใช้งานได้ในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="d50a8-103">If you no longer need your Azure subscription, you can cancel it in the Azure portal.</span></span> <span data-ttu-id="d50a8-104">การสมัครใช้งาน Azure สามารถยกเลิกได้โดยผู้ดูแลบัญชีหรือผู้ใช้ที่มีสิทธิ์เจ้าของในการสมัครใช้งานเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="d50a8-104">Azure subscriptions can only be canceled by the Account Administrator or by users with Owner rights on the subscription.</span></span>

1. <span data-ttu-id="d50a8-105">เลือกการสมัครใช้งานของคุณ[จากหน้าการสมัครใช้งานในพอร์ทัล Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="d50a8-105">Select your subscription from the [Subscriptions page in the Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="d50a8-106">เลือกการสมัครใช้งานที่คุณต้องการยกเลิก</span><span class="sxs-lookup"><span data-stu-id="d50a8-106">Select the subscription that you want to cancel.</span></span>
3. <span data-ttu-id="d50a8-107">**เลือก** ภาพรวม แล้วเลือก **ยกเลิก** การสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="d50a8-107">Select **Overview**, and then select **Cancel subscription**.</span></span>

<span data-ttu-id="d50a8-108">**จะเกิดอะไรขึ้นหลังจากที่ยกเลิกการสมัครใช้งานของฉัน**</span><span class="sxs-lookup"><span data-stu-id="d50a8-108">**What happens after I cancel my subscription?**</span></span>

<span data-ttu-id="d50a8-109">หลังจากที่คุณยกเลิก การเรียกเก็บเงินจะหยุดทันที</span><span class="sxs-lookup"><span data-stu-id="d50a8-109">After you cancel, billing is stopped immediately.</span></span> <span data-ttu-id="d50a8-110">อย่างไรก็ตาม อาจต้องใช้เวลาถึง 10 นาทีเพื่อให้การยกเลิกแสดงในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="d50a8-110">However, it can take up to 10 minutes for the cancellation to show in the portal.</span></span> <span data-ttu-id="d50a8-111">ถ้าคุณยกเลิกระหว่างระยะเวลาการเรียกเก็บเงิน เราจะส่งใบแจ้งหนี้ฉบับสุดท้ายในวันที่ใบแจ้งหนี้ทั่วไปของคุณหลังจากถึงช่วงเวลาสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="d50a8-111">If you cancel in the middle of a billing period, we send the final invoice on your typical invoice date after the period ends.</span></span>

<span data-ttu-id="d50a8-112">หลังจากที่คุณยกเลิก บริการของคุณถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="d50a8-112">After you cancel, your services are disabled.</span></span> <span data-ttu-id="d50a8-113">ซึ่งหมายความว่าเครื่องเสมือนของคุณไม่ได้จัดสรร ที่อยู่ IP ชั่วคราวจะว่าง และที่เก็บข้อมูลเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="d50a8-113">That means your virtual machines are de-allocated, temporary IP addresses are freed, and storage is read-only.</span></span>

<span data-ttu-id="d50a8-114">หลังจากยกเลิกการสมัครใช้งานแล้ว Microsoft จะรอ 30 -90 วันก่อนที่จะลบข้อมูลของคุณอย่างถาวร ในกรณีที่คุณต้องเข้าถึงข้อมูลหรือคุณเปลี่ยนใจ</span><span class="sxs-lookup"><span data-stu-id="d50a8-114">After your subscription is canceled, Microsoft waits 30 - 90 days before permanently deleting your data in case you need to access it or you change your mind.</span></span> <span data-ttu-id="d50a8-115">เราจะไม่เรียกเก็บเงินจากคุณในการรักษาข้อมูล</span><span class="sxs-lookup"><span data-stu-id="d50a8-115">We don't charge you for retaining the data.</span></span> <span data-ttu-id="d50a8-116">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [ศูนย์ความเชื่อถือของ Microsoft - วิธีที่เราจัดการ](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409)ข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="d50a8-116">To learn more, see [Microsoft Trust Center - How we manage your data](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409).</span></span>

<span data-ttu-id="d50a8-117">**ยกเลิกการสมัครใช้งาน Azure**</span><span class="sxs-lookup"><span data-stu-id="d50a8-117">**Cancel Azure Subscription**</span></span>

- [<span data-ttu-id="d50a8-118">ใครสามารถยกเลิกการสมัครใช้งานได้บ้าง</span><span class="sxs-lookup"><span data-stu-id="d50a8-118">Who can cancel a subscription?</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#who-can-cancel-a-subscription)
- [<span data-ttu-id="d50a8-119">จะเกิดอะไรขึ้นหลังจากการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="d50a8-119">What happens after the subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#what-happens-after-i-cancel-my-subscription)

<span data-ttu-id="d50a8-120">**เอกสารที่แนะนา**</span><span class="sxs-lookup"><span data-stu-id="d50a8-120">**Recommended Documents**</span></span>

- [<span data-ttu-id="d50a8-121">เปิดใช้งานการสมัครใช้งานใหม่</span><span class="sxs-lookup"><span data-stu-id="d50a8-121">Reactivate subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#reactivate-subscription)
- [<span data-ttu-id="d50a8-122">สลับการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="d50a8-122">Switch subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)