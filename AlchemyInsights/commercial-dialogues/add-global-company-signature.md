---
title: เพิ่มลายเซ็นของบริษัทส่วนกลางหรือข้อสงวนสิทธิ์ของผู้ใช้ทั้งหมด
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: cbd92f9c4a78139eac4e3672dd0632b173472757
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50508608"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="7541f-102">เพิ่มลายเซ็นของบริษัทส่วนกลางหรือข้อสงวนสิทธิ์ของผู้ใช้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7541f-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="7541f-103">เคล็ดลับ: ลายเซ็นแบบทั้งอุปกรณ์เรียกอีกอย่างว่าข้อสงวนสิทธิ์ ไม่ว่าจะรวมอะไรไว้อย่างไรก็ตาม</span><span class="sxs-lookup"><span data-stu-id="7541f-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="7541f-104">ในศูนย์การจัดการ ให้เลือก **ศูนย์การจัดการ**  >  **Exchange**</span><span class="sxs-lookup"><span data-stu-id="7541f-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="7541f-105">ภายใต้ลโฟลว์จดหมาย **ให้เลือก** กฎ</span><span class="sxs-lookup"><span data-stu-id="7541f-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="7541f-106">คลิกไอคอน **+** (เพิ่ม) แล้วเลือก **ใช้ข้อความปฏิเสธความรับผิดชอบ**</span><span class="sxs-lookup"><span data-stu-id="7541f-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="7541f-107">ตั้งชื่อกฎ</span><span class="sxs-lookup"><span data-stu-id="7541f-107">Give the rule a name.</span></span>
5. <span data-ttu-id="7541f-108">ภายใต้ ใช้กฎนี้ **ให้เลือก ใช้กับข้อความ** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7541f-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="7541f-109">ภายใต้ ให้ปล่อยข้อสงวน **สิทธิ์** ไว้ เลือก ผนวกข้อความปฏิเสธความรับผิดชอบ ไว้</span><span class="sxs-lookup"><span data-stu-id="7541f-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="7541f-110">คลิก **ใส่ข้อความ** แล้วพิมพ์ข้อความปฏิเสธความรับผิดชอบของคุณ</span><span class="sxs-lookup"><span data-stu-id="7541f-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="7541f-111">**คลิก เลือก\*\*\*\*หนึ่งตัวเลือก** เลือกตัวเลือก ตัดเป็นตัวเลือกย้อนกลับ **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="7541f-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="7541f-112">ซึ่งหมายความว่าถ้าไม่สามารถเพิ่มข้อสงวนสิทธิ์ได้เนื่องจากการเข้ารหัสลับหรือการตั้งค่าจดหมายอื่นๆ คําแถลงการณ์ปฏิเสธความรับผิดชอบจะถูกรวมเข้าในซองจดหมายข้อความ</span><span class="sxs-lookup"><span data-stu-id="7541f-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="7541f-113">ปล่อยให้ **ตรวจสอบกฎ** นี้ด้วยระดับความรุนแรงที่เลือกไว้</span><span class="sxs-lookup"><span data-stu-id="7541f-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="7541f-114">จากนั้นเลือก ต่่า กลาง หรือ สูง ที่จะใช้ในบันทึกข้อความ</span><span class="sxs-lookup"><span data-stu-id="7541f-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="7541f-115">เลือกบังคับใช้ เพื่อเปิดข้อความปฏิเสธความรับผิดชอบทันที ยกเว้นกรณีที่คุณต้องการทดสอบก่อน</span><span class="sxs-lookup"><span data-stu-id="7541f-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="7541f-116">เลือกตัวเลือก **เพิ่มเติม** เพื่อรวมเงื่อนไขหรือข้อยกเว้นเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7541f-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="7541f-117">เมื่อเสร็จแล้ว **ให้คลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="7541f-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="7541f-118">ต้องการความช่วยเหลือเพิ่มเติมใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="7541f-118">Need more help?</span></span> [<span data-ttu-id="7541f-119">ดูวิดีโอเกี่ยวกับการสร้างข้อสงวนสิทธิ์หรืออ่านบทความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7541f-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)