---
title: ตั้งค่ากฎเพื่อตอบกลับอีเมลขาเข้า
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "7254"
ms.openlocfilehash: 49b8aafe77aa6e31f8d724046c6fc0996294cc5d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525400"
---
# <a name="set-up-rules-to-reply-to-incoming-emails"></a><span data-ttu-id="4c384-102">ตั้งค่ากฎเพื่อตอบกลับอีเมลขาเข้า</span><span class="sxs-lookup"><span data-stu-id="4c384-102">Set up rules to reply to incoming emails</span></span>

<span data-ttu-id="4c384-103">ใช้ขั้นตอนต่อไปนี้เพื่อสร้างเทมเพลตเพื่อตอบกลับข้อความ จากนั้นตั้งค่า Outlook ให้ตอบกลับทุกข้อความที่คุณได้รับ</span><span class="sxs-lookup"><span data-stu-id="4c384-103">Use the following steps to create a template to reply to messages, and then set up Outlook to reply to every message you receive.</span></span>

1. <span data-ttu-id="4c384-104">ใน Outlook ให้สร้างข้อความอีเมลใหม่และใส่ชื่อเรื่องและเนื้อหาข้อความของเทมเพลตไม่อยู่ที่สํานักงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="4c384-104">In Outlook, create a new email message and enter a subject and message body for your out-of-office template.</span></span>
2. <span data-ttu-id="4c384-105">เลือก **ไฟล์ >บันทึก** เป็น</span><span class="sxs-lookup"><span data-stu-id="4c384-105">Select **File > Save As**.</span></span>
3. <span data-ttu-id="4c384-106">ในกล่องโต้ตอบ **บันทึกเป็น** จากเมนูดรอปดาวน์ **บันทึกเป็น** ชนิด ให้เลือก **เทมเพลต Outlook (\*.oft)**</span><span class="sxs-lookup"><span data-stu-id="4c384-106">In the **Save As** dialog box, from the **Save as type** drop-down, select **Outlook Template (\*.oft).**</span></span> <span data-ttu-id="4c384-107">ตั้งชื่อที่เหมาะสม แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="4c384-107">Give it an appropriate name, and then click **Save**.</span></span>
4. <span data-ttu-id="4c384-108">เลือก **กฎ**  >  **การจัดการไฟล์ &การแจ้งเตือน** ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4c384-108">Select the **File** > **Manage Rules & Alerts**.</span></span>
5. <span data-ttu-id="4c384-109">ในกล่องโต้ตอบ **กฎและ** การแจ้งเตือน บนแท็บ **กฎอีเมล** ให้คลิก **กฎ** ใหม่</span><span class="sxs-lookup"><span data-stu-id="4c384-109">In the **Rules and Alerts** dialog box, on the **E-mail Rules** tab, click **New Rule**.</span></span>
6. <span data-ttu-id="4c384-110">ในกล่องโต้ตอบ **ตัวช่วยสร้างกฎ** ภายใต้ เริ่มจาก **กฎที่ว่างเปล่า** ให้เลือก **ใช้กฎกับ** ข้อความที่ฉันได้รับ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="4c384-110">In the **Rules Wizard** dialog box, under **Start from a blank rule**, select **Apply rule on messages I receive**, and then click **Next**.</span></span>
7. <span data-ttu-id="4c384-111">เลือก ส่ง **ให้ฉันเท่านั้น แล้วคลิก\*\*\*\*ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="4c384-111">For the condition, select **sent only to me**, and then click **Next**.</span></span>
8. <span data-ttu-id="4c384-112">เลือกตอบกลับโดยใช้ **เทมเพลตที่ระบุ และ** ในบานหน้าต่างด้านล่าง ให้คลิก **เทมเพลต** ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="4c384-112">For the action, select **reply using a specific template**, and then in the bottom pane, click **a specific template**.</span></span>
9. <span data-ttu-id="4c384-113">ในกล่องโต้ตอบ **เลือกเทมเพลต** การตอบกลับ จากเมนูดร **อปดาวน์** ค้นหาใน **ให้เลือก เทมเพลตผู้ใช้ ในระบบ** ไฟล์</span><span class="sxs-lookup"><span data-stu-id="4c384-113">In the **Select a Reply Template** dialog box, from the **Look In** drop-down, select **User Templates in File System**.</span></span> <span data-ttu-id="4c384-114">เลือกเทมเพลตที่บันทึกไว้ก่อนหน้านี้ **แล้วคลิก** เปิด</span><span class="sxs-lookup"><span data-stu-id="4c384-114">Choose the previously saved template, and then click **Open**.</span></span>
10. <span data-ttu-id="4c384-115">ในบานหน้าต่างด้านล่างของกล่องโต้ตอบ คุณจะเห็นว่าไฟล์เทมเพลตถูกแทรก</span><span class="sxs-lookup"><span data-stu-id="4c384-115">In the bottom pane of the dialog box you'll see that the template file is inserted.</span></span> <span data-ttu-id="4c384-116">คลิกเสร็จสิ้น เพื่อปิดตัวช่วยสร้าง และ **กลับไปยังกล่องโต้ตอบ** กฎและการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="4c384-116">Click **Finish** to close the wizard and return to the **Rules and Alerts** dialog box.</span></span> <span data-ttu-id="4c384-117">โปรดสังเกตกฎ **ที่ส่งมาให้ฉันเท่านั้นที่สร้างขึ้น** ใหม่</span><span class="sxs-lookup"><span data-stu-id="4c384-117">Notice the newly created **sent only to me** rule.</span></span> <span data-ttu-id="4c384-118">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="4c384-118">Click **OK**.</span></span>
