---
title: ระบุการส่งต่ออีเมลภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716479"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="f2825-102">ระบุเมื่อมีการกําหนดค่าการส่งต่ออีเมลภายนอกบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="f2825-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="f2825-103">เมื่อผู้ใช้ Microsoft 365 กําหนดค่าการส่งต่ออีเมลภายนอกบนกล่องจดหมาย กิจกรรมถูกตรวจสอบเป็นส่วนหนึ่งของ cmdlet**กล่องจดหมายชุด**</span><span class="sxs-lookup"><span data-stu-id="f2825-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="f2825-104">คุณสามารถดูกิจกรรมโดยใช้การค้นหาบันทึกการตรวจสอบได้ในศูนย์การปฏิบัติตามกฎระเบียบความปลอดภัย&</span><span class="sxs-lookup"><span data-stu-id="f2825-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="f2825-105">เข้าสู่ระบบศูนย์[การปฏิบัติตาม&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f2825-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f2825-106">ไปที่หน้า**ค้นหาบันทึกการตรวจสอบ\*\*\*\*การค้นหา** > </span><span class="sxs-lookup"><span data-stu-id="f2825-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f2825-107">เลือกช่วงวันที่ในฟิลด์**วันที่เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="f2825-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f2825-108">คุณไม่จําเป็นต้องระบุชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f2825-108">You don't need to specify a username.</span></span> <span data-ttu-id="f2825-109">ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่า**เป็น แสดงผลลัพธ์สําหรับกิจกรรมทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="f2825-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="f2825-110">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="f2825-110">Click **Search**.</span></span>

<span data-ttu-id="f2825-111">ในผลลัพธ์ ให้คลิก**กรองผลลัพธ์**และชนิด**กล่องจดหมาย**ในกล่องตัวกรองกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="f2825-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="f2825-112">เลือกเรกคอร์ดการตรวจสอบในผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="f2825-112">Select an audit record in the results.</span></span> <span data-ttu-id="f2825-113">**ในรายละเอียด**ลอยคลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="f2825-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="f2825-114">คุณต้องดูรายละเอียดของเรกคอร์ดการตรวจสอบแต่ละเรกคอร์ดเพื่อดูว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมลหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f2825-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="f2825-115">**ObjectId:** ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="f2825-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="f2825-116">**พารามิเตอร์**:_การส่งต่อSmtpAddress_บ่งชี้ที่อยู่อีเมลเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="f2825-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="f2825-117">**UserId:** ผู้ใช้ที่กําหนดค่าการส่งต่ออีเมลบนกล่องจดหมายในฟิลด์**ObjectId**</span><span class="sxs-lookup"><span data-stu-id="f2825-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="f2825-118">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การกําหนดผู้ติดตั้งการส่งต่ออีเมลสําหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="f2825-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
