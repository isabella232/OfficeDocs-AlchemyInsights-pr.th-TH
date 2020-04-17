---
title: ข้อคิดเห็นใน Microsoft วางแผน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 682a00364063d395ef9053fc7f6d99a299451c1b
ms.sourcegitcommit: 1173501899034ad5f6a432311bc3f1091ead3efa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/16/2020
ms.locfileid: "43541882"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="45146-102">ข้อคิดเห็นใน Microsoft วางแผน</span><span class="sxs-lookup"><span data-stu-id="45146-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="45146-103">ข้อคิดเห็นสําหรับงานภายในแผนจะถูกเก็บไว้ในกล่องจดหมาย Exchange แบบออนไลน์สําหรับกลุ่ม Office 365 ที่เกี่ยวข้องกับแผน</span><span class="sxs-lookup"><span data-stu-id="45146-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Office 365 Group associated with the plan.</span></span>  <span data-ttu-id="45146-104">เมื่อคุณโพสต์ข้อคิดเห็นเกี่ยวกับงาน จะมีการส่งอีเมลแจ้งเตือนไปยังกล่องจดหมายเข้าของกลุ่ม และคุณจะได้รับอีเมลสําหรับข้อคิดเห็นที่ตามมาที่เกิดขึ้นในงานนั้น</span><span class="sxs-lookup"><span data-stu-id="45146-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="45146-105">ต่อไปนี้เป็นคําตอบของปัญหาทั่วไปที่เกี่ยวข้องกับข้อคิดเห็น</span><span class="sxs-lookup"><span data-stu-id="45146-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="45146-106">**ผู้ใช้ไม่ได้รับอีเมล**- ความคิดเห็นจะถูกส่งไปยังกล่องจดหมายของกลุ่มสําหรับกลุ่มที่แผนเป็นสมาชิกอยู่</span><span class="sxs-lookup"><span data-stu-id="45146-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="45146-107">สําหรับผู้ใช้ที่จะได้รับอีเมลกลุ่ม ควรกําหนดค่ากลุ่มเพื่อส่งการสนทนากลุ่มไปยังกล่องจดหมายของสมาชิก</span><span class="sxs-lookup"><span data-stu-id="45146-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="45146-108">**ข้อคิดเห็นไม่ได้รับการบันทึก**- ผู้ใช้ที่เพิ่มข้อคิดเห็นไม่มีสิทธิ์ในการส่งอีเมลไปยังกลุ่ม Office 365</span><span class="sxs-lookup"><span data-stu-id="45146-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Office 365 group.</span></span> <span data-ttu-id="45146-109">อ่าน[วิธีการทํางานของ Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสถานการณ์นี้</span><span class="sxs-lookup"><span data-stu-id="45146-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="45146-110">ข้อผิดพลาด**คุณไม่มีการเข้าถึง**จะแสดงขึ้น หรือ**ผู้ใช้ที่เป็นแขกไม่สามารถเพิ่มข้อคิดเห็น**- ผู้ใช้ที่เป็นแขกที่ไม่สามารถส่งอีเมล์ไปยังกล่องขาเข้าของกลุ่มอาจเห็นข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="45146-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="45146-111">เมื่อต้องการแก้ไข ให้แน่ใจว่า ผู้ใช้เป็นแขกมีที่อยู่อีเมลที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="45146-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="45146-112">**ผู้ใช้ที่ถูกลบจะได้รับอีเมล**- หากผู้ใช้ความคิดเห็นในงานก่อนที่จะถูกเอาออกจากแผนอีเมลเธรดจะมีผู้ใช้สําหรับความคิดเห็นที่ทําในแต่ละงาน</span><span class="sxs-lookup"><span data-stu-id="45146-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="45146-113">สําหรับข้อมูลรายละเอียดเกี่ยวกับข้อคิดเห็นเกี่ยวกับ Microsoft Planner ให้ดูที่วิธีการทํางานของ[Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)และ[ข้อคิดเห็นเกี่ยวกับงานใน Microsoft Planner](https://support.microsoft.com/en-us/office/comment-on-tasks-in-microsoft-planner-fd4aedde-7785-4cd0-96ee-122fbc9140e1)</span><span class="sxs-lookup"><span data-stu-id="45146-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/en-us/office/comment-on-tasks-in-microsoft-planner-fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
