---
title: ระบุการส่งต่ออีเมภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539120"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="862f3-102">ระบุเมื่อมีการกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="862f3-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="862f3-103">เมื่อผู้ใช้ Office 365 สามารถกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย กิจกรรมที่กำลังตรวจสอบเป็นส่วนหนึ่งของการ cmdlet**กล่องจดหมายชุด**</span><span class="sxs-lookup"><span data-stu-id="862f3-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="862f3-104">คุณสามารถดูกิจกรรมที่ใช้ค้นหาแฟ้มบันทึกการตรวจสอบใน & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="862f3-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="862f3-105">เข้าสู่ระบบไปยัง[ศูนย์การปฏิบัติตามกฎระเบียบ & ความปลอดภัย 365 Office](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="862f3-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="862f3-106">การ**ค้นหา**ไป > เพ**จค้นหาแฟ้มบันทึกการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="862f3-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="862f3-107">เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="862f3-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="862f3-108">คุณไม่จำเป็นเมื่อต้องการระบุชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="862f3-108">You don't need to specify a username.</span></span> <span data-ttu-id="862f3-109">ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเพื่อ**แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="862f3-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="862f3-110">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="862f3-110">Click **Search**.</span></span>

<span data-ttu-id="862f3-111">ในผลลัพธ์**ผลลัพธ์ของตัวกรอง**คลิก และพิมพ์การ**ตั้งค่าจดหมาย**ในกล่องตัวกรองกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="862f3-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="862f3-112">เลือกเรกคอร์ดที่มีตรวจสอบในผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="862f3-112">Select an audit record in the results.</span></span> <span data-ttu-id="862f3-113">ในเมนูลอยขึ้น**รายละเอียด**คลิ**กข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="862f3-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="862f3-114">คุณต้องดูที่รายละเอียดของแต่ละระเบียนตรวจสอบเพื่อตรวจสอบว่า กิจกรรมที่เกี่ยวข้องเพื่อส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="862f3-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="862f3-115">**ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="862f3-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="862f3-116">**พารามิเตอร์**: _ForwardingSmtpAddress_บ่งชี้ว่า อยู่อีเมลของเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="862f3-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="862f3-117">**UserId**: ผู้ใช้ที่กำหนดค่าไว้ส่งต่ออีเมลในกล่องจดหมายในฟิลด์**ObjectId**</span><span class="sxs-lookup"><span data-stu-id="862f3-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="862f3-118">สำหรับข้อมูลเพิ่มเติม ดู[Determining ที่ติดตั้งอีเมลที่ส่งต่อสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="862f3-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
