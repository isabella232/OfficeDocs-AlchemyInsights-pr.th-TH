---
title: ข้อคิดเห็นใน Microsoft Planner
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
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817659"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="90e1f-102">ข้อคิดเห็นใน Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="90e1f-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="90e1f-103">ข้อคิดเห็นของงานภายในแผนจะถูกเก็บไว้ในกล่องจดหมาย Exchange Online ของกลุ่ม Microsoft 365 ที่เกี่ยวข้องกับแผน</span><span class="sxs-lookup"><span data-stu-id="90e1f-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Microsoft 365 Group associated with the plan.</span></span>  <span data-ttu-id="90e1f-104">เมื่อคุณโพสต์ข้อคิดเห็นในงาน การแจ้งให้ทราบทางอีเมลจะถูกส่งไปยังกล่องขาเข้าของกลุ่ม และคุณจะได้รับอีเมลของแต่ละข้อคิดเห็นที่ตามมาเกี่ยวกับงานนั้น</span><span class="sxs-lookup"><span data-stu-id="90e1f-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="90e1f-105">ต่อไปนี้เป็นคําตอบของปัญหาทั่วไปที่เกี่ยวข้องกับข้อคิดเห็น:</span><span class="sxs-lookup"><span data-stu-id="90e1f-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="90e1f-106">**ผู้ใช้ไม่ได้รับอีเมล** - ข้อคิดเห็นจะถูกส่งไปยังกล่องขาเข้าของกลุ่มของกลุ่มที่แผนนั้นอยู่</span><span class="sxs-lookup"><span data-stu-id="90e1f-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="90e1f-107">เพื่อให้ผู้ใช้ได้รับอีเมลของกลุ่ม กลุ่มควรได้รับการกําหนดค่าให้ส่งการสนทนากลุ่มไปยังกล่องขาเข้าของสมาชิก</span><span class="sxs-lookup"><span data-stu-id="90e1f-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="90e1f-108">**ข้อคิดเห็นจะไม่ถูกบันทึก -** ผู้ใช้ที่เพิ่มข้อคิดเห็นไม่มีสิทธิ์ในการส่งอีเมลไปยังกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="90e1f-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Microsoft 365 group.</span></span> <span data-ttu-id="90e1f-109">อ่าน [วิธีการงานของ Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับสถานการณ์นี้</span><span class="sxs-lookup"><span data-stu-id="90e1f-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="90e1f-110">ข้อผิดพลาด **คุณไม่สามารถเข้าถึงแสดง** ได้อีกต่อไป หรือผู้ใช้ที่เป็นผู้ใช้ภายนอก **ไม่สามารถ** เพิ่มข้อคิดเห็นได้ ผู้ใช้ที่เป็นแขกที่ไม่สามารถส่งอีเมลไปยังกล่องขาเข้าของกลุ่มอาจเห็นข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="90e1f-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="90e1f-111">เมื่อต้องการแก้ไข ตรวจสอบให้แน่ใจว่าผู้ใช้ที่เป็นแขกมีที่อยู่อีเมลที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="90e1f-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="90e1f-112">**เอาผู้ใช้ออกแล้วจะได้รับอีเมล** - ถ้าผู้ใช้มีข้อคิดเห็นเกี่ยวกับงานก่อนที่จะถูกเอาออกจากแผน เธรดอีเมลจะรวมถึงผู้ใช้แต่ละคนที่มีข้อคิดเห็นแต่ละรายการในงาน</span><span class="sxs-lookup"><span data-stu-id="90e1f-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="90e1f-113">ดูข้อมูลโดยละเอียดเกี่ยวกับข้อคิดเห็นด้วย Microsoft Planner ดูวิธีการ[งานของ Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)และ[ข้อคิดเห็นเกี่ยวกับงานใน Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1)</span><span class="sxs-lookup"><span data-stu-id="90e1f-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
