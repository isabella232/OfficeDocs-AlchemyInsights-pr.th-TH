---
title: สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้ของคุณแชร์ปฏิทินกับบุคคลภายนอกองค์กรของคุณ
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
ms.openlocfilehash: 9ece122e0905d1afeb26e50fa0a5e049eee5c09d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806742"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="b474e-102">สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้ของคุณแชร์ปฏิทินกับบุคคลภายนอกองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b474e-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="b474e-103">จากแดชบอร์ดของศูนย์การจัดการ Microsoft ๓๖๕ให้**Admin**ไปที่  >  **Exchange**ของผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="b474e-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="b474e-104">ไปที่**organization**การ  >  **แชร์**องค์กร</span><span class="sxs-lookup"><span data-stu-id="b474e-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="b474e-105">ในมุมมองรายการภายใต้การ**แชร์แต่ละ**รายการให้คลิก**ใหม่**</span><span class="sxs-lookup"><span data-stu-id="b474e-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="b474e-106">ใน**นโยบายการแชร์ใหม่**ให้พิมพ์ชื่อที่จำง่ายสำหรับนโยบายการแชร์ในกล่อง**ชื่อนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="b474e-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="b474e-107">คลิก **เพิ่ม**  เพื่อกำหนดกฎการแชร์สำหรับนโยบาย</span><span class="sxs-lookup"><span data-stu-id="b474e-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="b474e-108">ใน **กฎการแชร์**ให้เลือกตัวเลือกใดตัวเลือกหนึ่งต่อไปนี้เพื่อระบุโดเมนที่คุณต้องการแชร์ด้วย:</span><span class="sxs-lookup"><span data-stu-id="b474e-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="b474e-109">**การแชร์กับโดเมนทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="b474e-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="b474e-110">**การแชร์กับโดเมนที่เฉพาะเจาะจง**</span><span class="sxs-lookup"><span data-stu-id="b474e-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="b474e-111">ถ้าคุณเลือกการ **แชร์กับโดเมนที่เฉพาะเจาะจง**ให้พิมพ์ชื่อของโดเมนที่คุณต้องการแชร์ด้วย</span><span class="sxs-lookup"><span data-stu-id="b474e-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="b474e-112">ถ้าคุณจำเป็นต้องใส่โดเมนมากกว่าหนึ่งโดเมนสำหรับนโยบายการแชร์นี้ให้บันทึกการตั้งค่าสำหรับโดเมนแรกแล้วแก้ไขกฎการแชร์เพื่อเพิ่มโดเมนเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b474e-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="b474e-113">เมื่อต้องการระบุข้อมูลที่สามารถแชร์ได้ให้เลือกกล่องกาเครื่องหมาย **แชร์โฟลเดอร์ปฏิทินของคุณ** แล้วเลือกตัวเลือกใดตัวเลือกหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b474e-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="b474e-114">**ข้อมูลสถานะว่าง/ไม่ว่างของปฏิทินที่มีเวลาเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="b474e-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="b474e-115">**ข้อมูลสถานะว่าง/ไม่ว่างของปฏิทินที่มีเวลาชื่อเรื่องและตำแหน่งที่ตั้ง**</span><span class="sxs-lookup"><span data-stu-id="b474e-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="b474e-116">**ข้อมูลการนัดหมายทั้งหมดในปฏิทินรวมถึงเวลาชื่อเรื่องตำแหน่งที่ตั้งและชื่อเรื่อง**</span><span class="sxs-lookup"><span data-stu-id="b474e-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="b474e-117">คลิก **บันทึก** เพื่อตั้งค่ากฎสำหรับนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="b474e-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="b474e-118">ถ้าคุณต้องการตั้งค่านโยบายการแชร์นี้เป็นนโยบายการแชร์เริ่มต้นใหม่สำหรับผู้ใช้ทั้งหมดในองค์กรของคุณให้เลือกกล่องกาเครื่องหมาย**ทำให้นโยบายนี้เป็นนโยบายการแชร์เริ่มต้นของฉัน**</span><span class="sxs-lookup"><span data-stu-id="b474e-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="b474e-119">คลิก **บันทึก** เพื่อสร้างนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="b474e-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="b474e-120">**สำหรับการทำความเข้าใจเกี่ยวกับหัวข้อนี้อย่างสมบูรณ์โปรดอ่าน:**</span><span class="sxs-lookup"><span data-stu-id="b474e-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="b474e-121">สร้างนโยบายการแชร์ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b474e-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="b474e-122">นำนโยบายการแชร์ไปใช้กับกล่องจดหมายใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b474e-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="b474e-123">ปรับเปลี่ยนปิดใช้งานหรือเอานโยบายการแชร์ออกใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b474e-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)