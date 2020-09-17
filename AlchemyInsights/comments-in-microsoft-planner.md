---
title: ข้อคิดเห็นใน Microsoft วางแผน
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
- "9001717"
- "3810"
ms.openlocfilehash: 048b63619256c1322837a06115f97127188aec6d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793597"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="092d5-102">ข้อคิดเห็นใน Microsoft วางแผน</span><span class="sxs-lookup"><span data-stu-id="092d5-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="092d5-103">ข้อคิดเห็นสำหรับงานภายในแผนจะถูกเก็บไว้ในกล่องจดหมาย Exchange Online สำหรับกลุ่ม Microsoft ๓๖๕ที่เชื่อมโยงกับแผน</span><span class="sxs-lookup"><span data-stu-id="092d5-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Microsoft 365 Group associated with the plan.</span></span>  <span data-ttu-id="092d5-104">เมื่อคุณโพสต์ข้อคิดเห็นในงานการแจ้งเตือนทางอีเมลจะถูกส่งไปยังกล่องจดหมายเข้าของกลุ่มและคุณจะได้รับอีเมลสำหรับข้อคิดเห็นที่ตามมาของแต่ละข้อคิดเห็นที่เกิดขึ้นในงานนั้น</span><span class="sxs-lookup"><span data-stu-id="092d5-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="092d5-105">ต่อไปนี้เป็นคำตอบของปัญหาทั่วไปที่เกี่ยวข้องกับข้อคิดเห็น:</span><span class="sxs-lookup"><span data-stu-id="092d5-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="092d5-106">**ผู้ใช้ไม่ได้รับอีเมลที่** ส่งข้อคิดเห็นจะถูกส่งไปยังกล่องจดหมายเข้าของกลุ่มสำหรับกลุ่มที่วางแผนเป็นสมาชิกอยู่</span><span class="sxs-lookup"><span data-stu-id="092d5-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="092d5-107">สำหรับผู้ใช้ในการรับอีเมลของกลุ่มกลุ่มควรได้รับการกำหนดค่าให้ส่งการสนทนากลุ่มไปยังกล่องจดหมายเข้าของสมาชิก</span><span class="sxs-lookup"><span data-stu-id="092d5-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="092d5-108">**ข้อคิดเห็นไม่ได้รับการบันทึก** -ผู้ใช้ที่เพิ่มข้อคิดเห็นไม่มีสิทธิ์ในการส่งอีเมลไปยังกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="092d5-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Microsoft 365 group.</span></span> <span data-ttu-id="092d5-109">อ่าน [วิธีการทำงานของ Microsoft วางแผน](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสถานการณ์สมมตินี้</span><span class="sxs-lookup"><span data-stu-id="092d5-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="092d5-110">ข้อผิดพลาดที่ **คุณไม่มีการเข้าถึง** จะแสดงขึ้นหรือ **ผู้ใช้ที่เป็นผู้เยี่ยมชมไม่สามารถเพิ่มข้อคิดเห็น** -ผู้ใช้ที่ไม่สามารถส่งอีเมลไปยังกล่องจดหมายเข้าของกลุ่มอาจเห็นข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="092d5-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="092d5-111">เมื่อต้องการแก้ไขให้ตรวจสอบให้แน่ใจว่าผู้ใช้ที่เป็นผู้เยี่ยมชมมีที่อยู่อีเมลที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="092d5-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="092d5-112">**ผู้ใช้ที่ถูกเอาออกจะได้รับอีเมล** -ถ้าข้อคิดเห็นของผู้ใช้ในงานก่อนที่จะถูกเอาออกจากแผนเธรดอีเมลที่มีผู้ใช้สำหรับแต่ละข้อคิดเห็นที่ทำบนงาน</span><span class="sxs-lookup"><span data-stu-id="092d5-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="092d5-113">สำหรับข้อมูลโดยละเอียดเกี่ยวกับข้อคิดเห็นที่มีการวางแผน Microsoft ให้ดูที่[วิธีการทำงานของ Microsoft วางแผน](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)และ[ข้อคิดเห็นเกี่ยวกับงานใน microsoft วางแผน](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1)</span><span class="sxs-lookup"><span data-stu-id="092d5-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
