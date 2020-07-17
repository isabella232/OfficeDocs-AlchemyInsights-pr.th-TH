---
title: สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้แชร์ปฏิทินกับบุคคลภายนอกองค์กรของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862210"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="65dbd-102">สร้างนโยบายการแชร์เพื่ออนุญาตให้ผู้ใช้แชร์ปฏิทินกับบุคคลภายนอกองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="65dbd-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="65dbd-103">จากแดชบอร์ดศูนย์การจัดการ Microsoft 365 ให้ไปที่**Admin**  >  **Exchange**ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="65dbd-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="65dbd-104">ไปที่**การแชร์องค์กร**  >  **sharing**</span><span class="sxs-lookup"><span data-stu-id="65dbd-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="65dbd-105">ในมุมมองรายการ ภายใต้**การแชร์บุคคล**ให้คลิก**สร้าง**</span><span class="sxs-lookup"><span data-stu-id="65dbd-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="65dbd-106">ใน**นโยบายการใช้ร่วมกันใหม่**ให้พิมพ์ชื่อที่เรียกง่ายสําหรับนโยบายการแชร์ในกล่อง**ชื่อนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="65dbd-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="65dbd-107">คลิก**add**เพื่อกําหนดกฎการแชร์สําหรับนโยบาย</span><span class="sxs-lookup"><span data-stu-id="65dbd-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="65dbd-108">ใน**กฎการแชร์**ให้เลือกตัวเลือกใดตัวเลือกหนึ่งต่อไปนี้เพื่อระบุโดเมนที่คุณต้องการแชร์ด้วย</span><span class="sxs-lookup"><span data-stu-id="65dbd-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="65dbd-109">**การแชร์กับโดเมนทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="65dbd-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="65dbd-110">**การแชร์กับโดเมนที่ระบุ**</span><span class="sxs-lookup"><span data-stu-id="65dbd-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="65dbd-111">ถ้าคุณเลือก**การแชร์กับโดเมนที่ระบุ**ให้พิมพ์ชื่อของโดเมนที่คุณต้องการแชร์ด้วย</span><span class="sxs-lookup"><span data-stu-id="65dbd-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="65dbd-112">หากคุณต้องการป้อนมากกว่าหนึ่งโดเมนสําหรับนโยบายการแชร์นี้ ให้บันทึกการตั้งค่าสําหรับโดเมนแรก จากนั้นแก้ไขกฎการแชร์เพื่อเพิ่มโดเมนเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="65dbd-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="65dbd-113">เมื่อต้องการระบุข้อมูลที่สามารถใช้ร่วมกันได้ ให้เลือกกล่องกาเครื่องหมาย**ใช้โฟลเดอร์ปฏิทินร่วมกัน**แล้วเลือกตัวเลือกใดตัวเลือกหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="65dbd-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="65dbd-114">**ข้อมูลว่าง/ไม่ว่างของปฏิทินที่มีเวลาเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="65dbd-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="65dbd-115">**ข้อมูลว่าง/ไม่ว่างของปฏิทินพร้อมเวลา เรื่อง และตําแหน่งที่ตั้ง**</span><span class="sxs-lookup"><span data-stu-id="65dbd-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="65dbd-116">**ข้อมูลการนัดหมายปฏิทินทั้งหมด รวมถึงเวลา เรื่อง ตําแหน่งที่ตั้ง และชื่อเรื่อง**</span><span class="sxs-lookup"><span data-stu-id="65dbd-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="65dbd-117">คลิก**บันทึก**เพื่อตั้งค่ากฎสําหรับนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="65dbd-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="65dbd-118">ถ้าคุณต้องการตั้งค่านโยบายการแชร์นี้เป็นนโยบายการแชร์เริ่มต้นใหม่สําหรับผู้ใช้ทั้งหมดในองค์กรของคุณ ให้เลือกกล่องกาเครื่องหมาย**กําหนดให้นโยบายนี้เป็นค่าเริ่มต้นของฉันใช้นโยบายการแชร์**</span><span class="sxs-lookup"><span data-stu-id="65dbd-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="65dbd-119">คลิก**บันทึก**เพื่อสร้างนโยบายการแชร์</span><span class="sxs-lookup"><span data-stu-id="65dbd-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="65dbd-120">**สําหรับความเข้าใจเต็มรูปแบบของหัวข้อนี้โปรดอ่าน :**</span><span class="sxs-lookup"><span data-stu-id="65dbd-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="65dbd-121">สร้างนโยบายการใช้ร่วมกันในการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="65dbd-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="65dbd-122">ใช้นโยบายการใช้ร่วมกันกับกล่องจดหมายในการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="65dbd-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="65dbd-123">ปรับเปลี่ยน ปิดใช้งาน หรือเอานโยบายที่ใช้ร่วมกันในการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="65dbd-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)