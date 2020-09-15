---
title: สร้างความสัมพันธ์ขององค์กรเพื่อให้ผู้ใช้ของคุณสามารถทำงานร่วมกับองค์กรอื่นได้
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
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712752"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="b989d-102">สร้างความสัมพันธ์ขององค์กรเพื่อให้ผู้ใช้ของคุณสามารถทำงานร่วมกับองค์กรอื่นได้</span><span class="sxs-lookup"><span data-stu-id="b989d-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="b989d-103">จากแดชบอร์ดของศูนย์การจัดการ Microsoft ๓๖๕ให้**Admin**ไปที่  >  **Exchange**ของผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="b989d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="b989d-104">ไปที่**organization**การ  >  **แชร์**องค์กร</span><span class="sxs-lookup"><span data-stu-id="b989d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="b989d-105">ภายใต้การ**แชร์องค์กร**ให้คลิก**ใหม่**</span><span class="sxs-lookup"><span data-stu-id="b989d-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="b989d-106">ใน **ความสัมพันธ์ขององค์กรใหม่**ในกล่อง **ชื่อความสัมพันธ์** ให้พิมพ์ชื่อที่จำง่ายสำหรับความสัมพันธ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="b989d-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="b989d-107">ในกล่อง **โดเมนเพื่อแชร์กับ** ให้พิมพ์โดเมนสำหรับ Office ๓๖๕ภายนอกหรือองค์กร Exchange ภายนอกที่คุณต้องการให้เห็นปฏิทินของคุณ</span><span class="sxs-lookup"><span data-stu-id="b989d-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="b989d-108">ถ้าคุณต้องการใส่โดเมนมากกว่าหนึ่งโดเมนให้แยกชื่อโดเมนด้วยเครื่องหมายจุลภาค</span><span class="sxs-lookup"><span data-stu-id="b989d-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="b989d-109">ตัวอย่างเช่น contoso.com, service.contoso.com</span><span class="sxs-lookup"><span data-stu-id="b989d-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="b989d-110">เลือกกล่องกาเครื่องหมาย **เปิดใช้งานการแชร์ข้อมูลว่าง/ไม่ว่างของปฏิทิน** เพื่อเปิดใช้งานการแชร์ปฏิทินกับโดเมนที่คุณอยู่ในรายการ</span><span class="sxs-lookup"><span data-stu-id="b989d-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="b989d-111">ตั้งค่าระดับการแชร์สำหรับข้อมูลว่าง/ไม่ว่างของปฏิทินและตั้งค่าผู้ใช้ที่สามารถแชร์ข้อมูลว่าง/ไม่ว่างของปฏิทินได้</span><span class="sxs-lookup"><span data-stu-id="b989d-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="b989d-112">เมื่อต้องการตั้งค่าระดับการเข้าถึงว่าง/ไม่ว่างให้เลือกอย่างใดอย่างหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b989d-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="b989d-113">**ข้อมูลสถานะว่าง/ไม่ว่างของปฏิทินที่มีเวลาเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="b989d-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="b989d-114">**ปฏิทินว่าง/ไม่ว่างกับเวลาหัวเรื่องและตำแหน่งที่ตั้ง**</span><span class="sxs-lookup"><span data-stu-id="b989d-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="b989d-115">เมื่อต้องการตั้งค่าผู้ใช้ที่จะแชร์ข้อมูลว่าง/ไม่ว่างของปฏิทินให้เลือกอย่างใดอย่างหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b989d-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="b989d-116">**ทุกคนในองค์กรของคุณ**</span><span class="sxs-lookup"><span data-stu-id="b989d-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="b989d-117">**กลุ่มความปลอดภัยที่ระบุ**</span><span class="sxs-lookup"><span data-stu-id="b989d-117">**A specified security group**</span></span>  

<span data-ttu-id="b989d-118">คลิก**เรียกดู**เพื่อเลือกกลุ่มความปลอดภัยจากรายการแล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="b989d-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="b989d-119">คลิก **บันทึก** เพื่อสร้างความสัมพันธ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="b989d-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="b989d-120">**หมายเหตุ:** การกำหนดค่าข้ามผู้เช่าไม่สนับสนุนการค้นหาที่ติดต่อส่วนบุคคลสำหรับการค้นหาว่าง/ไม่ว่าง</span><span class="sxs-lookup"><span data-stu-id="b989d-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="b989d-121">ผู้ติดต่อต้องรวมอยู่ในสมุดรายชื่อส่วนกลางสำหรับการค้นหาว่าง/ไม่ว่างในการทำงาน</span><span class="sxs-lookup"><span data-stu-id="b989d-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="b989d-122">**สำหรับการทำความเข้าใจเกี่ยวกับหัวข้อนี้อย่างสมบูรณ์โปรดอ่าน:**</span><span class="sxs-lookup"><span data-stu-id="b989d-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="b989d-123">สร้างความสัมพันธ์ขององค์กรใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b989d-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="b989d-124">ปรับเปลี่ยนความสัมพันธ์ขององค์กรใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b989d-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="b989d-125">เอาความสัมพันธ์ขององค์กรใน Exchange Online ออก</span><span class="sxs-lookup"><span data-stu-id="b989d-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
