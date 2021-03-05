---
title: อ่านบันทึกการตรวจสอบของเหตุการณ์ที่ถูกลบ
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483320"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="3de59-102">อ่านบันทึกการตรวจสอบของเหตุการณ์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="3de59-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="3de59-103">วิธีการมีดังนี้</span><span class="sxs-lookup"><span data-stu-id="3de59-103">Here's how to do this:</span></span>

1. <span data-ttu-id="3de59-104">ไปที่ศูนย์การรักษา[ความปลอดภัยของ office 365 &การปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="3de59-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="3de59-105">เลือก  >  [**การค้นหาบันทึกการตรวจสอบ**](https://go.microsoft.com/fwlink/?linkid=2103759)การค้นหา</span><span class="sxs-lookup"><span data-stu-id="3de59-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="3de59-106">ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดฟีเจอร์ นั้นเดินหน้าแล้วเปิดในตอนนี้</span><span class="sxs-lookup"><span data-stu-id="3de59-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="3de59-107">ถ้าฟีเจอร์ไม่ได้เปิดอยู่ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้</span><span class="sxs-lookup"><span data-stu-id="3de59-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="3de59-108">**เลือกกิจกรรม** แล้วค้นหา **กิจกรรมกล่องจดหมาย** Exchange</span><span class="sxs-lookup"><span data-stu-id="3de59-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="3de59-109">เลือกข้อความ **ที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ** และ **ย้ายข้อความไปยังตัวเลือกโฟลเดอร์** รายการที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="3de59-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="3de59-110">เมื่อคุณเสร็จสิ้น ให้คลิกภายนอกบานหน้าต่างเพื่อย่อ **บานหน้าต่างกิจกรรม**</span><span class="sxs-lookup"><span data-stu-id="3de59-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="3de59-111">ระบุช่วงวันที่ จากนั้น **ในกล่อง** ผู้ใช้ ให้เลือกชื่อผู้ใช้ของผู้ใช้ที่คุณต้องการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="3de59-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="3de59-112">คุณสามารถเลือกผู้ใช้ได้มากกว่าหนึ่งรายในครั้งเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="3de59-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="3de59-113">เลือกค้นหา</span><span class="sxs-lookup"><span data-stu-id="3de59-113">Select **Search**.</span></span> <span data-ttu-id="3de59-114">กิจกรรม **จะปรากฏขึ้นภายใต้** ผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="3de59-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="3de59-115">เมื่อต้องการดูรายละเอียด ให้เลือกกิจกรรม **จากนั้นเลือก** ข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3de59-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="3de59-116">ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ เช่น บรรทัดเรื่องและที่ตั้งของรายการเมื่อรายการถูกลบ จะแสดงอยู่ในเขตข้อมูล **AffectedItems**</span><span class="sxs-lookup"><span data-stu-id="3de59-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="3de59-117">คุณไม่สามารถคืนค่ารายการที่ถูกลบโดยใช้ฟีเจอร์บันทึกการตรวจสอบได้</span><span class="sxs-lookup"><span data-stu-id="3de59-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="3de59-118">เมื่อต้องการคืนค่ารายการที่ถูกลบ ให้ดู[กู้คืนรายการหรืออีเมลที่ถูกลบใน Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="3de59-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="3de59-119">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [ค้นหาบันทึกการตรวจสอบ Office 365 เพื่อแก้ไขปัญหาสถานการณ์](https://go.microsoft.com/fwlink/?linkid=2103944)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="3de59-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
