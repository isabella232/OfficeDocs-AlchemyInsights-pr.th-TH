---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662227"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="7f1bd-102">บันทึกการตรวจสอบของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="7f1bd-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="7f1bd-103">บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="7f1bd-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="7f1bd-104">SPO การตรวจสอบดั้งเดิมถูกโยกย้ายไปยังบันทึกการตรวจสอบแบบรวม (UAL)</span><span class="sxs-lookup"><span data-stu-id="7f1bd-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="7f1bd-105">ในตอนนี้รายงานการตรวจสอบแบบดั้งเดิมของ SPO ทั้งหมดจะได้รับการดำเนินการผ่าน UAL และจะมีการโยกย้ายสัญญาณการตรวจสอบแบบดั้งเดิมไปยัง UAL</span><span class="sxs-lookup"><span data-stu-id="7f1bd-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="7f1bd-106">การเปลี่ยนแปลงที่สำคัญ:</span><span class="sxs-lookup"><span data-stu-id="7f1bd-106">Key changes:</span></span>

* <span data-ttu-id="7f1bd-107">การตัดแต่งจะไม่พร้อมใช้งานเป็นความสามารถ</span><span class="sxs-lookup"><span data-stu-id="7f1bd-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="7f1bd-108">การเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7f1bd-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="7f1bd-109">อ้างอิงไปยัง [เอกสารนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) สำหรับรายการของเหตุการณ์ที่ตรวจสอบทั้งหมดที่พร้อมใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="7f1bd-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="7f1bd-110">ตัวเลือก **ตำแหน่งที่ตั้ง** ภายใต้ **รายงานแบบกำหนดเอง** จะไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7f1bd-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="7f1bd-111">ตัวเลือกการ **เปิดหรือการดาวน์โหลดเอกสาร** ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7f1bd-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="7f1bd-112">การกำหนดค่าการตั้งค่าการตรวจสอบสำหรับไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="7f1bd-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="7f1bd-113">บันทึกการตรวจสอบแบบครบวงจรของ SharePoint และ OneDrive จากการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="7f1bd-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="7f1bd-114">เปิด/ปิดการบันทึกการตรวจสอบแบบครบวงจร</span><span class="sxs-lookup"><span data-stu-id="7f1bd-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="7f1bd-115">ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="7f1bd-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="7f1bd-116">ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์ (s), สิทธิ์การใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="7f1bd-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="7f1bd-117">กิจกรรมของไฟล์และหน้า</span><span class="sxs-lookup"><span data-stu-id="7f1bd-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="7f1bd-118">กิจกรรมของโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="7f1bd-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="7f1bd-119">การแชร์และการร้องขอการเข้าถึงกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="7f1bd-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="7f1bd-120">กิจกรรมการซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="7f1bd-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="7f1bd-121">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="7f1bd-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="7f1bd-122">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกใช้เหตุการณ์เหล่านี้ให้ดู[ที่ค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="7f1bd-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
