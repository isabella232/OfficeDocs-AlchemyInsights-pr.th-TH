---
title: เพิ่มลายเซ็นของบริษัทส่วนกลางหรือข้อสงวนสิทธิ์ของผู้ใช้ทั้งหมด
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
- "1200009"
- "7310"
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483966"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="33ec0-102">เพิ่มลายเซ็นของบริษัทส่วนกลางหรือข้อสงวนสิทธิ์ของผู้ใช้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="33ec0-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="33ec0-103">เคล็ดลับ: ลายเซ็นแบบทั้งอุปกรณ์เรียกอีกอย่างว่าข้อสงวนสิทธิ์ ไม่ว่าจะรวมอะไรไว้อย่างไรก็ตาม</span><span class="sxs-lookup"><span data-stu-id="33ec0-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="33ec0-104">ในศูนย์การจัดการ ให้เลือก **ศูนย์การจัดการ**  >  **Exchange**</span><span class="sxs-lookup"><span data-stu-id="33ec0-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="33ec0-105">ภายใต้ลโฟลว์จดหมาย **ให้เลือก** กฎ</span><span class="sxs-lookup"><span data-stu-id="33ec0-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="33ec0-106">คลิกไอคอน **+** (เพิ่ม) แล้วเลือก **ใช้ข้อความปฏิเสธความรับผิดชอบ**</span><span class="sxs-lookup"><span data-stu-id="33ec0-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="33ec0-107">ตั้งชื่อกฎ</span><span class="sxs-lookup"><span data-stu-id="33ec0-107">Give the rule a name.</span></span>
5. <span data-ttu-id="33ec0-108">ภายใต้ ใช้กฎนี้ **ให้เลือก ใช้กับข้อความ** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="33ec0-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="33ec0-109">ภายใต้ ให้เลือกตัวเลือก ผนวกข้อ **สงวน** สิทธิ์ ทิ้งไว้</span><span class="sxs-lookup"><span data-stu-id="33ec0-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="33ec0-110">คลิก **ใส่ข้อความ** แล้วพิมพ์ข้อความปฏิเสธความรับผิดชอบของคุณ</span><span class="sxs-lookup"><span data-stu-id="33ec0-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="33ec0-111">**คลิก เลือก\*\*\*\*หนึ่งตัวเลือก** เลือกตัวเลือก ตัดเป็นตัวเลือกย้อนกลับ **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="33ec0-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="33ec0-112">ซึ่งหมายความว่าถ้าไม่สามารถเพิ่มข้อสงวนสิทธิ์ได้เนื่องจากการเข้ารหัสลับหรือการตั้งค่าจดหมายอื่นๆ คําแถลงการณ์ปฏิเสธความรับผิดชอบจะถูกรวมเข้าในซองจดหมายข้อความ</span><span class="sxs-lookup"><span data-stu-id="33ec0-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="33ec0-113">ปล่อยให้ **ตรวจสอบกฎ** นี้ด้วยระดับความรุนแรงที่เลือกไว้</span><span class="sxs-lookup"><span data-stu-id="33ec0-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="33ec0-114">จากนั้นเลือก ต่่า กลาง หรือ สูง ที่จะใช้ในบันทึกข้อความ</span><span class="sxs-lookup"><span data-stu-id="33ec0-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="33ec0-115">เลือกบังคับใช้ เพื่อเปิดข้อความปฏิเสธความรับผิดชอบทันที ยกเว้นกรณีที่คุณต้องการทดสอบก่อน</span><span class="sxs-lookup"><span data-stu-id="33ec0-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="33ec0-116">เลือกตัวเลือก **เพิ่มเติม** เพื่อใส่เงื่อนไขหรือข้อยกเว้นเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="33ec0-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="33ec0-117">เมื่อเสร็จแล้ว **ให้คลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="33ec0-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="33ec0-118">ต้องการความช่วยเหลือเพิ่มเติมใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="33ec0-118">Need more help?</span></span> [<span data-ttu-id="33ec0-119">ดูวิดีโอเกี่ยวกับการสร้างข้อสงวนสิทธิ์หรืออ่านบทความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="33ec0-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)