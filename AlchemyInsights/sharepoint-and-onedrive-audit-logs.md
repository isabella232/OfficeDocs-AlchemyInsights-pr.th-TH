---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509619"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="7b1b8-102">บันทึกการตรวจสอบของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="7b1b8-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="7b1b8-103">บันทึกการตรวจสอบแบบคลาสสิคของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="7b1b8-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="7b1b8-104">การตรวจสอบแบบดั้งเดิมของ SPO ถูกโยกย้ายไปบันทึกการตรวจสอบโดยรวม (UAL)</span><span class="sxs-lookup"><span data-stu-id="7b1b8-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="7b1b8-105">รายงานการตรวจสอบ SPO แบบดั้งเดิมทั้งหมดจะได้รับพลังงานผ่าน UAL และสัญญาณการตรวจสอบแบบดั้งเดิมได้ถูกย้ายไปยัง UAL</span><span class="sxs-lookup"><span data-stu-id="7b1b8-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="7b1b8-106">การเปลี่ยนแปลงที่สําคัญ:</span><span class="sxs-lookup"><span data-stu-id="7b1b8-106">Key changes:</span></span>

* <span data-ttu-id="7b1b8-107">การตัดแต่งไม่สามารถใช้ได้เป็นความสามารถ</span><span class="sxs-lookup"><span data-stu-id="7b1b8-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="7b1b8-108">การเลือกเหตุการณ์เฉพาะเพื่อตรวจสอบจะไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7b1b8-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="7b1b8-109">อ้างอิง[ถึงเอกสารนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)สําหรับรายการเหตุการณ์ที่ตรวจสอบทั้งหมดที่มีให้เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="7b1b8-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="7b1b8-110">ตัวเลือก**ตําแหน่งที่ตั้ง**ภายใต้**รายงานที่กําหนดเอง**ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7b1b8-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="7b1b8-111">ตัวเลือก**การเปิดหรือการดาวน์โหลดเหตุการณ์เอกสาร**ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7b1b8-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="7b1b8-112">การกําหนดค่าการตั้งค่าการตรวจสอบสําหรับไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="7b1b8-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="7b1b8-113">บันทึกการตรวจสอบโดยรวมแบบสมัยใหม่ของ SharePoint และ OneDrive จากการปฏิบัติตามข้อกําหนด</span><span class="sxs-lookup"><span data-stu-id="7b1b8-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="7b1b8-114">เปิด/ปิดการบันทึกการตรวจสอบโดยรวม</span><span class="sxs-lookup"><span data-stu-id="7b1b8-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="7b1b8-115">ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="7b1b8-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="7b1b8-116">ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์โฟลเดอร์ผู้ใช้สิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="7b1b8-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="7b1b8-117">กิจกรรมไฟล์และเพจ</span><span class="sxs-lookup"><span data-stu-id="7b1b8-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="7b1b8-118">กิจกรรมโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="7b1b8-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="7b1b8-119">การแชร์และการเข้าถึงกิจกรรมคําขอ</span><span class="sxs-lookup"><span data-stu-id="7b1b8-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="7b1b8-120">กิจกรรมการซิงโครไนส์</span><span class="sxs-lookup"><span data-stu-id="7b1b8-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="7b1b8-121">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="7b1b8-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="7b1b8-122">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกเหตุการณ์เหล่านี้ ให้ดูที่[การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="7b1b8-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
