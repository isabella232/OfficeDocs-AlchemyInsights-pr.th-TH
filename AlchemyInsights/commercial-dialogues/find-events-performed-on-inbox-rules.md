---
title: ค้นหาเหตุการณ์ที่ปฏิบัติตามกฎกล่องจดหมายเข้า
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483706"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="77f1a-102">ค้นหาเหตุการณ์ที่กิจกรรมในกฎกล่องจดหมายเข้า</span><span class="sxs-lookup"><span data-stu-id="77f1a-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="77f1a-103">เมื่อกฎกล่องจดหมายเข้าถูกสร้าง เปลี่ยนแปลง หรือลบ เหตุการณ์จะถูกบันทึกในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="77f1a-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="77f1a-104">ต่อไปนี้เป็นวิธีตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="77f1a-104">Here's how to review them:</span></span>

1. <span data-ttu-id="77f1a-105">ไปที่ศูนย์การรักษา[ความปลอดภัยของ office 365 &การปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="77f1a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="77f1a-106">เลือก>การค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="77f1a-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="77f1a-107">ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดการตรวจสอบ ให้เดินหน้าแล้วเปิดตอนนี้</span><span class="sxs-lookup"><span data-stu-id="77f1a-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="77f1a-108">ถ้าไม่ได้เปิดฟีเจอร์นี้ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้</span><span class="sxs-lookup"><span data-stu-id="77f1a-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="77f1a-109">เลือกเขตข้อมูลกิจกรรมและค้นหากิจกรรมกล่องจดหมาย Exchange แล้วเลือก New-InboxRuleกฎกล่องจดหมายเข้าจาก Outlook Web App</span><span class="sxs-lookup"><span data-stu-id="77f1a-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="77f1a-110">เมื่อคุณเสร็จสิ้น ให้คลิกภายนอกบานหน้าต่างเพื่อย่อบานหน้าต่างกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="77f1a-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="77f1a-111">ระบุช่วงวันที่ จากนั้นในเขตข้อมูลผู้ใช้ ให้เลือกชื่อผู้ใช้ของผู้ใช้ที่คุณต้องการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="77f1a-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="77f1a-112">คุณสามารถเลือกผู้ใช้ได้มากกว่าหนึ่งรายในครั้งเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="77f1a-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="77f1a-113">เลือกค้นหา</span><span class="sxs-lookup"><span data-stu-id="77f1a-113">Select Search.</span></span> <span data-ttu-id="77f1a-114">กิจกรรมจะปรากฏขึ้นภายใต้ผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="77f1a-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="77f1a-115">เมื่อต้องการดูรายละเอียด ให้เลือกกิจกรรม จากนั้นเลือกข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="77f1a-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="77f1a-116">ภายใต้ส่วน พารามิเตอร์ คุณสามารถดูชื่อของกฎ ชุดเงื่อนไข และการแอคชันที่กฎนั้นจะต้องใช้</span><span class="sxs-lookup"><span data-stu-id="77f1a-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="77f1a-117">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู ค้นหาบันทึกการตรวจสอบ Office 365 เพื่อแก้ไขปัญหาสถานการณ์ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="77f1a-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>