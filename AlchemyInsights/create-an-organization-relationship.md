---
title: สร้างความสัมพันธ์องค์กรเพื่ออนุญาตให้ผู้ใช้ของคุณร่วมงานกับองค์กรอื่นได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816147"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="09d8b-102">สร้างความสัมพันธ์องค์กรเพื่ออนุญาตให้ผู้ใช้ของคุณร่วมงานกับองค์กรอื่นได้</span><span class="sxs-lookup"><span data-stu-id="09d8b-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="09d8b-103">จากแดชบอร์ดศูนย์การจัดการ Microsoft 365 ให้ไปที่ **Admin**  >  **Exchange**</span><span class="sxs-lookup"><span data-stu-id="09d8b-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="09d8b-104">ไปที่ **การแชร์**  >  **องค์กร**</span><span class="sxs-lookup"><span data-stu-id="09d8b-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="09d8b-105">ภายใต้ **การแชร์** องค์กร **ให้คลิก** ใหม่</span><span class="sxs-lookup"><span data-stu-id="09d8b-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="09d8b-106">**ในความสัมพันธ์องค์กรใหม่** ในกล่อง **ชื่อความสัมพันธ์** ให้พิมพ์ชื่อที่ง่ายของความสัมพันธ์องค์กร</span><span class="sxs-lookup"><span data-stu-id="09d8b-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="09d8b-107">ในกล่อง **โดเมนที่จะแชร์กับ** ให้พิมพ์โดเมนของ Office 365 ภายนอก หรือ Exchange ภายในองค์กรที่คุณต้องการดูปฏิทินของคุณ</span><span class="sxs-lookup"><span data-stu-id="09d8b-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="09d8b-108">ถ้าคุณต้องการใส่โดเมนมากกว่าหนึ่งโดเมน ให้แยกชื่อโดเมนด้วยเครื่องหมายจุลภาค</span><span class="sxs-lookup"><span data-stu-id="09d8b-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="09d8b-109">ตัวอย่างเช่น contoso.com service.contoso.com</span><span class="sxs-lookup"><span data-stu-id="09d8b-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="09d8b-110">เลือกกล่องกา **เครื่องหมาย เปิดใช้งานการแชร์ข้อมูลว่าง/ไม่ว่าง** ในปฏิทิน เพื่อเปิดการแชร์ปฏิทินกับโดเมนที่คุณแสดงอยู่ในรายการ</span><span class="sxs-lookup"><span data-stu-id="09d8b-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="09d8b-111">ตั้งค่าระดับการแชร์ข้อมูลว่าง/ไม่ว่างของปฏิทิน และตั้งค่าว่าผู้ใช้สามารถแชร์ข้อมูลว่าง/ไม่ว่างของปฏิทินได้</span><span class="sxs-lookup"><span data-stu-id="09d8b-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="09d8b-112">เมื่อต้องการตั้งค่าระดับการเข้าถึงว่าง/ไม่ว่าง ให้เลือกอย่างใดอย่างหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="09d8b-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="09d8b-113">**ข้อมูลว่าง/ไม่ว่างของปฏิทินที่มีเวลาเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="09d8b-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="09d8b-114">**ว่าง/ไม่ว่างของปฏิทินที่มีเวลา ชื่อเรื่อง และที่ตั้ง**</span><span class="sxs-lookup"><span data-stu-id="09d8b-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="09d8b-115">เมื่อต้องการตั้งค่าผู้ใช้ที่จะแชร์ข้อมูลว่าง/ไม่ว่างในปฏิทิน ให้เลือกอย่างใดอย่างหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="09d8b-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="09d8b-116">**ทุกคนในองค์กรของคุณ**</span><span class="sxs-lookup"><span data-stu-id="09d8b-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="09d8b-117">**กลุ่มความปลอดภัยที่ระบุ**</span><span class="sxs-lookup"><span data-stu-id="09d8b-117">**A specified security group**</span></span>  

<span data-ttu-id="09d8b-118">**คลิก** เรียกดู เพื่อเลือกกลุ่มความปลอดภัยจากรายการ **จากนั้นคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="09d8b-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="09d8b-119">**คลิก** บันทึก เพื่อสร้างความสัมพันธ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="09d8b-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="09d8b-120">**หมายเหตุ:** การกําหนดค่าข้ามผู้เช่าไม่สนับสนุนที่ติดต่อส่วนบุคคลในการค้นหาว่าง/ไม่ว่าง</span><span class="sxs-lookup"><span data-stu-id="09d8b-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="09d8b-121">ที่ติดต่อต้องถูกรวมไว้ในสมุดรายชื่อส่วนกลางเพื่อให้การค้นหาว่าง/ไม่ว่างสามารถใช้งาน</span><span class="sxs-lookup"><span data-stu-id="09d8b-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="09d8b-122">**เพื่อความเข้าใจในหัวข้อนี้อย่างเต็มรูปแบบ โปรดอ่าน:**</span><span class="sxs-lookup"><span data-stu-id="09d8b-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="09d8b-123">สร้างความสัมพันธ์องค์กรใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="09d8b-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="09d8b-124">ปรับเปลี่ยนความสัมพันธ์องค์กรใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="09d8b-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="09d8b-125">เอาความสัมพันธ์องค์กรใน Exchange Online ออก</span><span class="sxs-lookup"><span data-stu-id="09d8b-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
