---
title: รายงานSharePointการตรวจสอบแบบคลาสสิก
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
ms.openlocfilehash: f84a86331ffe714ffb5154d55608a91725a2fbfb
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233625"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="88bdf-102">SharePointและOneDriveบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="88bdf-102">SharePoint and OneDrive audit logs</span></span>

* [<span data-ttu-id="88bdf-103">เปิด/ปิดการบันทึกการตรวจสอบแบบครบวงจร</span><span class="sxs-lookup"><span data-stu-id="88bdf-103">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="88bdf-104">ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ โฟลเดอร์ ผู้ใช้ สิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="88bdf-104">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="88bdf-105">กิจกรรมของไฟล์และหน้า</span><span class="sxs-lookup"><span data-stu-id="88bdf-105">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="88bdf-106">กิจกรรมของโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="88bdf-106">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="88bdf-107">กิจกรรมการแชร์และการร้องขอการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="88bdf-107">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="88bdf-108">กิจกรรมการซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="88bdf-108">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="88bdf-109">กิจกรรมการจัดการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="88bdf-109">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="88bdf-110">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="88bdf-110">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="88bdf-111">การตรวจสอบแบบดั้งเดิมของ SPO ถูกโยกย้ายไปยังบันทึกการตรวจสอบแบบครบวงจร (UAL)</span><span class="sxs-lookup"><span data-stu-id="88bdf-111">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="88bdf-112">รายงานการตรวจสอบแบบดั้งเดิมของ SPO ทั้งหมดถูกขับเคลื่อนผ่าน UAL และสัญญาณการตรวจสอบแบบดั้งเดิมถูกโยกย้ายไปยัง UAL</span><span class="sxs-lookup"><span data-stu-id="88bdf-112">All SPO legacy audit reports are powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span> <span data-ttu-id="88bdf-113">For more information, see [Configure audit data for a site collection](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2).</span><span class="sxs-lookup"><span data-stu-id="88bdf-113">For more information, see [Configure audit data for a site collection](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2).</span></span>
