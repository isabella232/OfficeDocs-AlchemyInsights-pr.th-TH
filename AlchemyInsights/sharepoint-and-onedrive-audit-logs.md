---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992637"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="47ca7-102">บันทึกการตรวจสอบ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="47ca7-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="47ca7-103">บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="47ca7-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="47ca7-104">การตรวจสอบดั้งเดิมของที่ได้รับการโยกย้ายไปยังบันทึกการตรวจสอบรวม (นวล)</span><span class="sxs-lookup"><span data-stu-id="47ca7-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="47ca7-105">ขณะนี้รายงานการตรวจสอบแบบดั้งเดิมของที่ได้รับการสนับสนุนทั้งหมดจะถูกใช้งานผ่านทางด้านหน้าและมีการย้ายสัญญาณการตรวจสอบแบบดั้งเดิมไปยัง</span><span class="sxs-lookup"><span data-stu-id="47ca7-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="47ca7-106">การเปลี่ยนแปลงที่สำคัญ:</span><span class="sxs-lookup"><span data-stu-id="47ca7-106">Key changes:</span></span>

* <span data-ttu-id="47ca7-107">การตัดแต่งไม่สามารถใช้ได้เป็นความสามารถ</span><span class="sxs-lookup"><span data-stu-id="47ca7-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="47ca7-108">การเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบไม่สามารถใช้ได้</span><span class="sxs-lookup"><span data-stu-id="47ca7-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="47ca7-109">อ้างอิงถึง[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สำหรับรายการที่สมบูรณ์ของเหตุการณ์ที่ตรวจสอบพร้อมใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="47ca7-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="47ca7-110">ตัวเลือกที่**ตั้ง**ภายใต้**รายงานที่กำหนดเอง**ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="47ca7-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="47ca7-111">ตัวเลือกการ**เปิดหรือดาวน์โหลดเอกสาร**เหตุการณ์ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="47ca7-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="47ca7-112">กำหนดการตั้งค่าการตรวจสอบสำหรับชุดเก็บรวบรวมไซต์</span><span class="sxs-lookup"><span data-stu-id="47ca7-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="47ca7-113">SharePoint และ OneDrive ทันสมัยรวมบันทึกการตรวจสอบจากการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="47ca7-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="47ca7-114">เปิด/ปิดการบันทึกการตรวจสอบรวม</span><span class="sxs-lookup"><span data-stu-id="47ca7-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="47ca7-115">ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="47ca7-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="47ca7-116">ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์, ผู้ใช้ (s), สิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="47ca7-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="47ca7-117">กิจกรรมของแฟ้มและเพจ</span><span class="sxs-lookup"><span data-stu-id="47ca7-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="47ca7-118">กิจกรรมโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="47ca7-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="47ca7-119">การแชร์และการเข้าถึงกิจกรรมการร้องขอ</span><span class="sxs-lookup"><span data-stu-id="47ca7-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="47ca7-120">กิจกรรมการซิงโครไนส์</span><span class="sxs-lookup"><span data-stu-id="47ca7-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="47ca7-121">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="47ca7-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="47ca7-122">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการค้นคืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="47ca7-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
