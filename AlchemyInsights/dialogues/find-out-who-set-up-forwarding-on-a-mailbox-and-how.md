---
title: ค้นหาว่าใครตั้งค่าการส่งต่อบนกล่องจดหมาย และวิธีการ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429997"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="59b20-102">ค้นหาว่าใครตั้งค่าการส่งต่อบนกล่องจดหมาย และวิธีการ</span><span class="sxs-lookup"><span data-stu-id="59b20-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="59b20-103">ถ้าการส่งต่อภายนอกถูกตั้งค่าบนกล่องจดหมาย กิจกรรมจะถูกตรวจสอบเป็นส่วนหนึ่งของSet-Mailbox cmdlet</span><span class="sxs-lookup"><span data-stu-id="59b20-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="59b20-104">ต่อไปนี้เป็นวิธีการค้นหากิจกรรมในบันทึกการตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="59b20-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="59b20-105">ไปที่ศูนย์การรักษา[ความปลอดภัยของ office 365 &การปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="59b20-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="59b20-106">เลือก >  **การค้นหาบันทึกการตรวจสอบ** การค้นหา</span><span class="sxs-lookup"><span data-stu-id="59b20-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="59b20-107">ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดการตรวจสอบ ให้เดินหน้าแล้วเปิดตอนนี้</span><span class="sxs-lookup"><span data-stu-id="59b20-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="59b20-108">ถ้าไม่ได้เปิดฟีเจอร์นี้ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้</span><span class="sxs-lookup"><span data-stu-id="59b20-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="59b20-109">ตรวจสอบให้แน่ใจว่า **เขตข้อมูลกิจกรรม** ถูกตั้งค่าเป็น **แสดงผลลัพธ์กิจกรรมทั้งหมด** (ค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="59b20-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="59b20-110">ระบุช่วงวันที่</span><span class="sxs-lookup"><span data-stu-id="59b20-110">Specify the date range.</span></span> <span data-ttu-id="59b20-111">คุณไม่าเป็นต้องระบุชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="59b20-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="59b20-112">เลือกค้นหา</span><span class="sxs-lookup"><span data-stu-id="59b20-112">Select **Search**.</span></span> <span data-ttu-id="59b20-113">กิจกรรม **จะปรากฏขึ้นภายใต้** ผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="59b20-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="59b20-114">เลือก **กรอง** ผลลัพธ์ แล้วใส่ **Set-mailbox** **ในเขตข้อมูล** ตัวกรองกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="59b20-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="59b20-115">ซึ่งส่งกลับ **กิจกรรม Set-Mailbox** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="59b20-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="59b20-116">เมื่อต้องการดูรายละเอียด ให้เลือกกิจกรรม **จากนั้นเลือก** ข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="59b20-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="59b20-117">ภายใต้ **พารามิเตอร์** คุณจะเห็นที่อยู่อีเมลการส่งต่อที่ตั้งค่าบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="59b20-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="59b20-118">**UserID** จะแสดงผู้ใช้ที่ตั้งค่าการส่งต่อภายนอกบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="59b20-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="59b20-119">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [ค้นหาบันทึกการตรวจสอบ Office 365 เพื่อแก้ไขปัญหาสถานการณ์](https://go.microsoft.com/fwlink/?linkid=2103944)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="59b20-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>