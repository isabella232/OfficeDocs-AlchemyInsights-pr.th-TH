---
title: ค้นหาที่อยู่ IP ในบันทึกการตรวจสอบ
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429793"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="01e0a-102">ค้นหาที่อยู่ IP ในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="01e0a-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="01e0a-103">ที่อยู่ IP ที่สอดคล้องกับกิจกรรมที่โดยผู้ใช้หรือผู้ดูแลระบบจะแสดงในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="01e0a-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="01e0a-104">ข้อมูลลูกค้าจะได้รับการบันทึกด้วย</span><span class="sxs-lookup"><span data-stu-id="01e0a-104">The client information is also logged.</span></span> <span data-ttu-id="01e0a-105">ต่อไปนี้เป็นวิธีระบุที่อยู่ IP:</span><span class="sxs-lookup"><span data-stu-id="01e0a-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="01e0a-106">ไปที่ศูนย์การรักษา[ความปลอดภัยของ office 365 &การปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="01e0a-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="01e0a-107">เลือก  >  **[การค้นหาบันทึกการตรวจสอบ](https://go.microsoft.com/fwlink/?linkid=2103759)** การค้นหา</span><span class="sxs-lookup"><span data-stu-id="01e0a-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="01e0a-108">ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดการตรวจสอบ ให้เดินหน้าแล้วเปิดตอนนี้</span><span class="sxs-lookup"><span data-stu-id="01e0a-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="01e0a-109">ถ้าไม่ได้เปิดใช้งานฟีเจอร์นี้ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้</span><span class="sxs-lookup"><span data-stu-id="01e0a-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="01e0a-110">ถ้าคุณสนใจกิจกรรมที่เฉพาะเจาะจง **ให้เลือกกิจกรรมจากรายการ** กิจกรรม มิฉะนั้น ตามค่าเริ่มต้น กิจกรรมทั้งหมดจะถูกส่งกลับให้กับผู้ใช้ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="01e0a-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="01e0a-111">โปรดทราบว่าบางกิจกรรมอาจไม่พร้อมใช้งาน **ให้เลือกจากเมนูกิจกรรม** อย่างไรก็ตาม รายการตรวจสอบเหล่านั้นจะถูกส่งกลับถ้า **เลือก แสดงผลลัพธ์ของกิจกรรมทั้งหมด** (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="01e0a-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="01e0a-112">ระบุช่วงวันที่ และ **ในเขตข้อมูล** ผู้ใช้ ให้เลือกชื่อผู้ใช้ของผู้ใช้ที่คุณต้องการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="01e0a-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="01e0a-113">เลือกค้นหา</span><span class="sxs-lookup"><span data-stu-id="01e0a-113">Select **Search**.</span></span> <span data-ttu-id="01e0a-114">กิจกรรม **จะปรากฏขึ้นภายใต้** ผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="01e0a-114">The activities appear under **Results**.</span></span> <span data-ttu-id="01e0a-115">คุณสามารถดูที่อยู่ IP ของแต่ละกิจกรรมได้</span><span class="sxs-lookup"><span data-stu-id="01e0a-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="01e0a-116">เมื่อต้องการดูรายละเอียด ให้เลือกกิจกรรม **จากนั้นเลือก** ข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="01e0a-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="01e0a-117">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู ค้นหาบันทึก [การตรวจสอบ Office 365 เพื่อแก้ไขปัญหาสถานการณ์](https://go.microsoft.com/fwlink/?linkid=2103944)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="01e0a-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>