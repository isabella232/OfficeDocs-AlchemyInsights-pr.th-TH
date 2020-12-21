---
title: เพิ่มวิธีการชำระเงิน-ขั้นตอนที่แนะนำ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004284"
- "7649"
ms.openlocfilehash: 51045d4b35833ed72097d75ff1720a9d2604d196
ms.sourcegitcommit: 728800af2fe596756bcd2280f85451926a3e987c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722006"
---
# <a name="add-payment-method---recommended-steps"></a><span data-ttu-id="e1584-102">เพิ่มวิธีการชำระเงิน-ขั้นตอนที่แนะนำ</span><span class="sxs-lookup"><span data-stu-id="e1584-102">Add payment method - recommended steps</span></span>

<span data-ttu-id="e1584-103">คุณต้องมีสิทธิ์การใช้งานทั้งผู้ดูแลระบบบัญชีผู้ใช้และเจ้าของการสมัครใช้งานเพื่อยกเลิกการสมัครใช้งานในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="e1584-103">You must have the privileges of both an account administrator and the subscription owner to cancel a subscription in Azure portal.</span></span> 

<span data-ttu-id="e1584-104">เมื่อต้องการยกเลิกการสมัครใช้งานในพอร์ทัล Azure ให้คลิก [ยกเลิกการสมัคร](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ใช้งาน azure และจะเปลี่ยนเส้นทางให้คุณไปยังหน้าการ **สมัคร** ใช้งานใน Azure portal เพื่อเลือกและยกเลิกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e1584-104">To cancel a subscription in Azure portal, click [Cancel Azure subscription](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and that will redirect you to the **subscription** page in Azure portal to select and cancel the subscription.</span></span> 

<span data-ttu-id="e1584-105">**จะเกิดอะไรขึ้นหลังจากที่ฉันยกเลิกการสมัครใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="e1584-105">**What happens after I cancel the subscription?**</span></span> 

<span data-ttu-id="e1584-106">เมื่อยกเลิกการสมัครใช้งานการเรียกเก็บเงินจะหยุดทำงานทันที</span><span class="sxs-lookup"><span data-stu-id="e1584-106">Upon cancellation of the subscription, billing is stopped immediately.</span></span> <span data-ttu-id="e1584-107">อย่างไรก็ตามอาจใช้เวลานานถึง10นาทีสำหรับสถานะการยกเลิกที่จะแสดงในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="e1584-107">However, it can take up to 10 minutes for the cancellation status to display in the Azure portal.</span></span> <span data-ttu-id="e1584-108">Microsoft จะส่งใบแจ้งหนี้สุดท้ายในใบแจ้งหนี้ของเดือนถัดไปสำหรับปริมาณการใช้หรือการซื้อบางส่วน</span><span class="sxs-lookup"><span data-stu-id="e1584-108">Microsoft will send the final invoice on the next month’s invoice for any partial consumption or purchase.</span></span> <span data-ttu-id="e1584-109">บริการที่ทำงานในการสมัครใช้งานถูกปิดใช้งานเมื่อการยกเลิกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e1584-109">The services running in the subscription are disabled upon subscription cancellation.</span></span> <span data-ttu-id="e1584-110">นั่นหมายความว่าเครื่องเสมือนได้รับการจัดสรรแล้วที่อยู่ IP ชั่วคราวจะว่างและที่เก็บข้อมูลจะกลายเป็น **แบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="e1584-110">That means the virtual machines are de-allocated, temporary IP addresses are freed, and storage becomes **read-only**.</span></span> 

<span data-ttu-id="e1584-111">หลังจากยกเลิกการสมัครใช้งานแล้ว Microsoft จะรอ30-90 วันก่อนที่จะลบข้อมูลอย่างถาวรในกรณีที่คุณจำเป็นต้องเข้าถึงหรือคุณเปลี่ยนใจ</span><span class="sxs-lookup"><span data-stu-id="e1584-111">After the subscription is cancelled, Microsoft waits for 30-90 days before permanently deleting the data in case you need to access it or you change your mind.</span></span> <span data-ttu-id="e1584-112">Microsoft ไม่คิดค่าใช้จ่ายสำหรับการรักษาข้อมูล</span><span class="sxs-lookup"><span data-stu-id="e1584-112">Microsoft does not charge for retaining the data.</span></span> <span data-ttu-id="e1584-113">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่ศูนย์ความเชื่อถือของไมโครซอฟท์-วิธีที่เราจัดการข้อมูลของคุณ](https://www.microsoft.com/trust-center/privacy/data-management#leave)</span><span class="sxs-lookup"><span data-stu-id="e1584-113">For more information, see [Microsoft Trust Center - How we manage your data](https://www.microsoft.com/trust-center/privacy/data-management#leave).</span></span>



