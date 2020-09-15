---
title: ระบุการส่งต่ออีเมลภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696316"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="fa6cc-102">ระบุเวลาที่การส่งต่ออีเมลภายนอกถูกกำหนดค่าในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="fa6cc-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="fa6cc-103">เมื่อผู้ใช้ Microsoft ๓๖๕กำหนดค่าการส่งต่ออีเมลภายนอกในกล่องจดหมายกิจกรรมจะถูกตรวจสอบโดยเป็นส่วนหนึ่งของ cmdlet**กล่องจดหมายตั้งค่า**</span><span class="sxs-lookup"><span data-stu-id="fa6cc-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="fa6cc-104">คุณสามารถดูกิจกรรมโดยใช้การค้นหาบันทึกการตรวจสอบในศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="fa6cc-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="fa6cc-105">ลงชื่อเข้าใช้[ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="fa6cc-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fa6cc-106">ไปที่หน้า**Search**  >  **ค้นหาบันทึกการตรวจสอบ**การค้นหา</span><span class="sxs-lookup"><span data-stu-id="fa6cc-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="fa6cc-107">เลือกช่วงวันที่ในเขตข้อมูลวันที่**เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="fa6cc-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="fa6cc-108">คุณไม่จำเป็นต้องระบุชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="fa6cc-108">You don't need to specify a username.</span></span> <span data-ttu-id="fa6cc-109">ตรวจสอบว่าเขตข้อมูล **กิจกรรม** ถูกตั้งค่าให้ **แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="fa6cc-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="fa6cc-110">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="fa6cc-110">Click **Search**.</span></span>

<span data-ttu-id="fa6cc-111">ในผลลัพธ์ให้คลิก **ตัวกรองผลลัพธ์** และชนิดของ **กล่องจดหมายตั้งค่า** ในกล่องตัวกรองกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="fa6cc-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="fa6cc-112">เลือกระเบียนการตรวจสอบในผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="fa6cc-112">Select an audit record in the results.</span></span> <span data-ttu-id="fa6cc-113">ในเมนู**รายละเอียด**ให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="fa6cc-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="fa6cc-114">คุณต้องดูรายละเอียดของระเบียนการตรวจสอบแต่ละระเบียนเพื่อกำหนดว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมลหรือไม่</span><span class="sxs-lookup"><span data-stu-id="fa6cc-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="fa6cc-115">**ObjectId**: ค่านามแฝงของกล่องจดหมายที่ได้รับการปรับเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="fa6cc-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="fa6cc-116">**พารามิเตอร์**: _ForwardingSmtpAddress_ ระบุที่อยู่อีเมลของเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="fa6cc-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="fa6cc-117">**UserId**: ผู้ใช้ที่กำหนดค่าการส่งต่ออีเมลในกล่องจดหมายในเขตข้อมูล**ObjectId**</span><span class="sxs-lookup"><span data-stu-id="fa6cc-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="fa6cc-118">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การกำหนดผู้ที่ตั้งค่าการส่งต่ออีเมลสำหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="fa6cc-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
