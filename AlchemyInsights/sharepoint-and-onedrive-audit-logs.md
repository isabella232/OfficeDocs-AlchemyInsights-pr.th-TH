---
title: รายงานบันทึกการตรวจสอบของ SharePoint แบบคลาสสิก
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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741984"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f5a5f-102">บันทึกการตรวจสอบ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="f5a5f-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f5a5f-103">บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="f5a5f-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f5a5f-104">การตรวจสอบแบบดั้งเดิมของ SPO ถูกโยกย้ายไปยังบันทึกการตรวจสอบรวม (UAL)</span><span class="sxs-lookup"><span data-stu-id="f5a5f-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f5a5f-105">รายงานการตรวจสอบแบบดั้งเดิมของ SPO ทั้งหมดจะถูกขับเคลื่อนผ่าน UAL และสัญญาณการตรวจสอบแบบดั้งเดิมได้ถูกย้ายไปยัง UAL</span><span class="sxs-lookup"><span data-stu-id="f5a5f-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f5a5f-106">การเปลี่ยนแปลงที่สําคัญ:</span><span class="sxs-lookup"><span data-stu-id="f5a5f-106">Key changes:</span></span>

* <span data-ttu-id="f5a5f-107">การตัดแต่งไม่พร้อมใช้งานเป็นความสามารถ</span><span class="sxs-lookup"><span data-stu-id="f5a5f-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f5a5f-108">การเลือกเหตุการณ์เฉพาะที่จะตรวจสอบไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f5a5f-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f5a5f-109">โปรดดู[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สําหรับรายการเหตุการณ์ที่ตรวจสอบทั้งหมดที่พร้อมใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f5a5f-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f5a5f-110">ตัวเลือก**ตําแหน่ง**ภายใต้**รายงานที่กําหนดเอง**จะไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f5a5f-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f5a5f-111">ตัวเลือก**การเปิดหรือดาวน์โหลด**เอกสารเหตุการณ์ไม่สามารถใช้ได้</span><span class="sxs-lookup"><span data-stu-id="f5a5f-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f5a5f-112">การกําหนดค่าการตรวจสอบการตั้งค่าสําหรับไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="f5a5f-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f5a5f-113">บันทึกการตรวจสอบแบบครบวงจรสมัยใหม่ของ SharePoint และ OneDrive จากการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="f5a5f-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f5a5f-114">เปิด/ปิดการบันทึกการตรวจสอบรวม</span><span class="sxs-lookup"><span data-stu-id="f5a5f-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f5a5f-115">ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="f5a5f-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f5a5f-116">ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของแฟ้ม, โฟลเดอร์, user(s),</span><span class="sxs-lookup"><span data-stu-id="f5a5f-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f5a5f-117">กิจกรรมไฟล์และเพจ</span><span class="sxs-lookup"><span data-stu-id="f5a5f-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f5a5f-118">กิจกรรมโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="f5a5f-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f5a5f-119">กิจกรรมการแชร์และการร้องขอการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="f5a5f-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f5a5f-120">กิจกรรมการซิงโครไนส์</span><span class="sxs-lookup"><span data-stu-id="f5a5f-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f5a5f-121">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="f5a5f-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f5a5f-122">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกเหตุการณ์เหล่านี้ ให้ดูที่[การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="f5a5f-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
