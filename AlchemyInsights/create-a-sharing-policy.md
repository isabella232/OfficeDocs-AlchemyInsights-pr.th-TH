---
title: สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้ของคุณแชร์ปฏิทินของพวกเขากับบุคคลภายนอกองค์กรของคุณ
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
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816291"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="73ba8-102">สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้ของคุณแชร์ปฏิทินของพวกเขากับบุคคลภายนอกองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="73ba8-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="73ba8-103">จากแดชบอร์ดศูนย์การจัดการ Microsoft 365 ให้ไปที่ **Admin**  >  **Exchange**</span><span class="sxs-lookup"><span data-stu-id="73ba8-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="73ba8-104">ไปที่ **การแชร์**  >  **องค์กร**</span><span class="sxs-lookup"><span data-stu-id="73ba8-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="73ba8-105">ในมุมมองรายการ ภายใต้ **การแชร์แต่ละรายการ\*\*\*\*ให้คลิก** ใหม่</span><span class="sxs-lookup"><span data-stu-id="73ba8-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="73ba8-106">ใน **นโยบายการแชร์** ใหม่ ให้พิมพ์ชื่อที่ที่เป็นมิตรเกี่ยวกับนโยบายการแชร์ในกล่อง **ชื่อ** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="73ba8-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="73ba8-107">คลิก **เพิ่ม**  เพื่อกําหนดกฎการแชร์ของนโยบาย</span><span class="sxs-lookup"><span data-stu-id="73ba8-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="73ba8-108">**ใน กฎ** การแชร์ ให้เลือกหนึ่งในตัวเลือกต่อไปนี้เพื่อระบุโดเมนที่คุณต้องการแชร์ด้วย:</span><span class="sxs-lookup"><span data-stu-id="73ba8-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="73ba8-109">**การแชร์กับโดเมนทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="73ba8-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="73ba8-110">**การแชร์กับโดเมนที่ระบุ**</span><span class="sxs-lookup"><span data-stu-id="73ba8-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="73ba8-111">ถ้าคุณเลือก **การแชร์กับโดเมน** ที่ระบุ ให้พิมพ์ชื่อของโดเมนที่คุณต้องการแชร์ด้วย</span><span class="sxs-lookup"><span data-stu-id="73ba8-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="73ba8-112">ถ้าคุณต้องการใส่โดเมนมากกว่าหนึ่งโดเมนในนโยบายการแชร์นี้ ให้บันทึกการตั้งค่าของโดเมนแรก จากนั้นแก้ไขกฎการแชร์เพื่อเพิ่มโดเมนเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="73ba8-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="73ba8-113">เมื่อต้องการระบุข้อมูลที่สามารถแชร์ได้ ให้เลือกกล่อง **กาเครื่องหมาย** แชร์โฟลเดอร์ปฏิทินของคุณ แล้วเลือกตัวเลือกใดตัวเลือกหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="73ba8-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="73ba8-114">**ข้อมูลว่าง/ไม่ว่างของปฏิทินที่มีเวลาเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="73ba8-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="73ba8-115">**ข้อมูลว่าง/ไม่ว่างของปฏิทินที่มีเวลา ชื่อเรื่อง และที่ตั้ง**</span><span class="sxs-lookup"><span data-stu-id="73ba8-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="73ba8-116">**ข้อมูลการนัดหมายในปฏิทินทั้งหมด รวมถึงเวลา ชื่อเรื่อง สถานที่ และชื่อเรื่อง**</span><span class="sxs-lookup"><span data-stu-id="73ba8-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="73ba8-117">คลิกบันทึก เพื่อตั้งค่ากฎของนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="73ba8-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="73ba8-118">ถ้าคุณต้องการตั้งค่านโยบายการแชร์นี้เป็นนโยบายการแชร์เริ่มต้นใหม่ให้กับผู้ใช้ทุกคนในองค์กรของคุณ ให้เลือกกล่องกาเครื่องหมาย ตั้งให้นโยบายนี้เป็น **นโยบายการแชร์เริ่มต้น** ของฉัน</span><span class="sxs-lookup"><span data-stu-id="73ba8-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="73ba8-119">**คลิก** บันทึก เพื่อสร้างนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="73ba8-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="73ba8-120">**เพื่อความเข้าใจในหัวข้อนี้อย่างเต็มรูปแบบ โปรดอ่าน:**</span><span class="sxs-lookup"><span data-stu-id="73ba8-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="73ba8-121">สร้างนโยบายการแชร์ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="73ba8-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="73ba8-122">ปรับใช้นโยบายการแชร์กับกล่องจดหมายใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="73ba8-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="73ba8-123">ปรับเปลี่ยน ปิดใช้งาน หรือเอานโยบายการแชร์ใน Exchange Online ออก</span><span class="sxs-lookup"><span data-stu-id="73ba8-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)