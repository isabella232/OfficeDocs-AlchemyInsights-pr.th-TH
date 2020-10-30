---
title: ยกเลิกการสมัครใช้งานใน Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003797"
- "6786"
ms.openlocfilehash: f85608446c8b230753dccd06ee5b5ea36aed7802
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807939"
---
# <a name="cancel-subscription"></a><span data-ttu-id="6853b-102">ยกเลิกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6853b-102">Cancel Subscription</span></span>

<span data-ttu-id="6853b-103">เฉพาะผู้ดูแลระบบบัญชีผู้ใช้หรือเจ้าของที่อยู่บนการสมัครใช้งานคุณสามารถยกเลิกการสมัครใช้งาน Azure ของคุณในพอร์ทัล Azure ได้ถ้าคุณไม่ต้องการการสมัครใช้งานอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="6853b-103">Only Account Administrator or Owner right on the subscription You can cancel your Azure subscription in the Azure portal if you no longer need the subscription.</span></span> <span data-ttu-id="6853b-104">ทำตามขั้นตอนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="6853b-104">Follow the below steps.</span></span>

1. <span data-ttu-id="6853b-105">เลือกการสมัครใช้งานของคุณจากหน้าการสมัครใช้งาน[ในพอร์ทัล Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="6853b-105">Select your subscription from the [Subscriptions page in the Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="6853b-106">เลือกการสมัครใช้งานที่คุณต้องการยกเลิก</span><span class="sxs-lookup"><span data-stu-id="6853b-106">Select the subscription that you want to cancel.</span></span>
3. <span data-ttu-id="6853b-107">เลือก **ภาพรวม** แล้วเลือก **ยกเลิกการสมัคร** ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6853b-107">Select **Overview** , and then select **Cancel subscription** .</span></span>

<span data-ttu-id="6853b-108">**จะเกิดอะไรขึ้นหลังจากที่ฉันยกเลิกการสมัครใช้งานของฉัน**</span><span class="sxs-lookup"><span data-stu-id="6853b-108">**What happens after I cancel my subscription?**</span></span>

<span data-ttu-id="6853b-109">หลังจากที่คุณยกเลิกการเรียกเก็บเงินจะหยุดทำงานทันที</span><span class="sxs-lookup"><span data-stu-id="6853b-109">After you cancel, billing is stopped immediately.</span></span> <span data-ttu-id="6853b-110">อย่างไรก็ตามอาจใช้เวลาถึง10นาทีในการยกเลิกเพื่อแสดงในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="6853b-110">However, it can take up to 10 minutes for the cancellation to show in the portal.</span></span> <span data-ttu-id="6853b-111">ถ้าคุณยกเลิกตรงกลางของระยะเวลาการเรียกเก็บเงินเราจะส่งใบแจ้งหนี้สุดท้ายในวันที่ใบแจ้งหนี้ทั่วไปของคุณหลังจากสิ้นสุดระยะเวลา</span><span class="sxs-lookup"><span data-stu-id="6853b-111">If you cancel in the middle of a billing period, we send the final invoice on your typical invoice date after the period ends.</span></span>

<span data-ttu-id="6853b-112">หลังจากที่คุณยกเลิกบริการของคุณจะถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6853b-112">After you cancel, your services are disabled.</span></span> <span data-ttu-id="6853b-113">นั่นหมายความว่าเครื่องเสมือนของคุณได้รับการจัดสรรแล้วที่อยู่ IP ชั่วคราวจะว่างเปล่าและที่เก็บข้อมูลเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="6853b-113">That means your virtual machines are de-allocated, temporary IP addresses are freed, and storage is read-only.</span></span>

<span data-ttu-id="6853b-114">หลังจากที่การสมัครใช้งานของคุณถูกยกเลิกแล้ว Microsoft จะรอ 30-90 วันก่อนที่จะลบข้อมูลของคุณอย่างถาวรในกรณีที่คุณจำเป็นต้องเข้าถึงหรือเปลี่ยนใจของคุณ</span><span class="sxs-lookup"><span data-stu-id="6853b-114">After your subscription is canceled, Microsoft waits 30 - 90 days before permanently deleting your data in case you need to access it or you change your mind.</span></span> <span data-ttu-id="6853b-115">เราไม่คิดค่าบริการสำหรับการเก็บรักษาข้อมูล</span><span class="sxs-lookup"><span data-stu-id="6853b-115">We don't charge you for retaining the data.</span></span> <span data-ttu-id="6853b-116">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[ศูนย์ความเชื่อถือของไมโครซอฟท์-วิธีที่เราจัดการข้อมูลของคุณ](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="6853b-116">To learn more, see [Microsoft Trust Center - How we manage your data](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409).</span></span>

<span data-ttu-id="6853b-117">**ยกเลิกการสมัครใช้งาน Azure**</span><span class="sxs-lookup"><span data-stu-id="6853b-117">**Cancel Azure Subscription**</span></span>

- [<span data-ttu-id="6853b-118">ใครสามารถยกเลิกการสมัครใช้งานได้บ้าง</span><span class="sxs-lookup"><span data-stu-id="6853b-118">Who can cancel a subscription?</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#who-can-cancel-a-subscription)
- [<span data-ttu-id="6853b-119">จะเกิดอะไรขึ้นหลังจากการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6853b-119">What happens after the subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#what-happens-after-i-cancel-my-subscription)

<span data-ttu-id="6853b-120">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="6853b-120">**Recommended Documents**</span></span>

- [<span data-ttu-id="6853b-121">เปิดใช้งานการสมัครใช้งานใหม่</span><span class="sxs-lookup"><span data-stu-id="6853b-121">Reactivate subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#reactivate-subscription)
- [<span data-ttu-id="6853b-122">สลับการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6853b-122">Switch subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)