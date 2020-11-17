---
title: วิธีการยกเลิกการสมัครใช้งาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003797"
- "6836"
ms.openlocfilehash: af5b16a55afd7e26601e8ffa6288a72c94b9b1fb
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089059"
---
# <a name="how-to-cancel-a-subscription"></a><span data-ttu-id="00f94-102">วิธีการยกเลิกการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="00f94-102">How to cancel a subscription</span></span>

<span data-ttu-id="00f94-103">คุณสามารถยกเลิกการสมัครใช้งาน Azure ในพอร์ทัล Azure ได้ก็ต่อเมื่อคุณเป็นผู้ดูแลระบบบัญชีผู้ใช้หรือการสมัครใช้งานเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="00f94-103">You can cancel an Azure subscription in the Azure portal only if you are the Account Administrator or the subscription.</span></span> <span data-ttu-id="00f94-104">ทำตามขั้นตอนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="00f94-104">Follow the below steps.</span></span>

1. <span data-ttu-id="00f94-105">เลือกการสมัครใช้งานของคุณจากหน้าการสมัครใช้งาน[ในพอร์ทัล Azure](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="00f94-105">Select your subscription from the [Subscriptions page in the Azure portal](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="00f94-106">เลือกการสมัครใช้งานที่คุณต้องการยกเลิก</span><span class="sxs-lookup"><span data-stu-id="00f94-106">Select the subscription that you want to cancel.</span></span>
3. <span data-ttu-id="00f94-107">เลือก **ภาพรวม** แล้วเลือก **ยกเลิกการสมัคร** ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="00f94-107">Select **Overview**, and then select **Cancel subscription**.</span></span>

<span data-ttu-id="00f94-108">**จะเกิดอะไรขึ้นหลังจากที่ฉันยกเลิกการสมัครใช้งานของฉัน**</span><span class="sxs-lookup"><span data-stu-id="00f94-108">**What happens after I cancel my subscription?**</span></span>

<span data-ttu-id="00f94-109">หลังจากที่คุณยกเลิกการสมัครใช้งานการเรียกเก็บเงินของคุณจะหยุดทำงานทันที</span><span class="sxs-lookup"><span data-stu-id="00f94-109">After you cancel your subscription, billing is stopped immediately.</span></span> <span data-ttu-id="00f94-110">อย่างไรก็ตามอาจใช้เวลาถึง10นาทีในการยกเลิกเพื่อแสดงในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="00f94-110">However, it can take up to 10 minutes for the cancellation to show in the portal.</span></span> <span data-ttu-id="00f94-111">ถ้าคุณยกเลิกการสมัครใช้งานของคุณในช่วงเวลาการเรียกเก็บเงินเราจะส่งใบแจ้งหนี้สุดท้ายในวันที่ใบแจ้งหนี้ทั่วไปของคุณหลังจากสิ้นสุดระยะเวลา</span><span class="sxs-lookup"><span data-stu-id="00f94-111">If you cancel your subscription in the middle of a billing period, we send the final invoice on your typical invoice date after the period ends.</span></span>

<span data-ttu-id="00f94-112">หลังจากที่คุณยกเลิกบริการของคุณจะถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="00f94-112">After you cancel, your services are disabled.</span></span> <span data-ttu-id="00f94-113">นั่นหมายความว่าเครื่องเสมือนของคุณได้รับการจัดสรรแล้วที่อยู่ IP ชั่วคราวจะว่างเปล่าและที่เก็บข้อมูลเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="00f94-113">That means your virtual machines are de-allocated, temporary IP addresses are freed, and storage is read-only.</span></span>

<span data-ttu-id="00f94-114">หลังจากที่การสมัครใช้งานของคุณถูกยกเลิกแล้ว Microsoft จะรอ30-90 วันก่อนที่จะลบข้อมูลของคุณอย่างถาวรในกรณีที่คุณจำเป็นต้องเข้าถึงหรือเปลี่ยนใจของคุณ</span><span class="sxs-lookup"><span data-stu-id="00f94-114">After your subscription is canceled, Microsoft waits for 30-90 days before permanently deleting your data in case you need to access it or you change your mind.</span></span> <span data-ttu-id="00f94-115">เราไม่คิดค่าบริการสำหรับการเก็บรักษาข้อมูล</span><span class="sxs-lookup"><span data-stu-id="00f94-115">We don't charge you for retaining the data.</span></span> <span data-ttu-id="00f94-116">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ศูนย์ความเชื่อถือของไมโครซอฟท์-วิธีที่เราจัดการข้อมูลของคุณ](https://www.microsoft.com/trust-center/privacy/data-management#leave)</span><span class="sxs-lookup"><span data-stu-id="00f94-116">For more information, see [Microsoft Trust Center - How we manage your data](https://www.microsoft.com/trust-center/privacy/data-management#leave).</span></span>

