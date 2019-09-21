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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068042"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8f1f7-102">บันทึกการตรวจสอบ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="8f1f7-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="8f1f7-103">**SharePoint และ OneDrive ทันสมัยรวมบันทึกการตรวจสอบจากการปฏิบัติตามกฎระเบียบ**</span><span class="sxs-lookup"><span data-stu-id="8f1f7-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="8f1f7-104">เปิด/ปิดการบันทึกการตรวจสอบรวม</span><span class="sxs-lookup"><span data-stu-id="8f1f7-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8f1f7-105">ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="8f1f7-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="8f1f7-106">ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์, ผู้ใช้ (s), สิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="8f1f7-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="8f1f7-107">กิจกรรมของแฟ้มและเพจ</span><span class="sxs-lookup"><span data-stu-id="8f1f7-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="8f1f7-108">กิจกรรมโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="8f1f7-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="8f1f7-109">การแชร์และการเข้าถึงกิจกรรมการร้องขอ</span><span class="sxs-lookup"><span data-stu-id="8f1f7-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="8f1f7-110">กิจกรรมการซิงโครไนส์</span><span class="sxs-lookup"><span data-stu-id="8f1f7-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="8f1f7-111">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="8f1f7-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="8f1f7-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการค้นคืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="8f1f7-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="8f1f7-113">**บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint**</span><span class="sxs-lookup"><span data-stu-id="8f1f7-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="8f1f7-114">เราย้ายการตรวจสอบที่สืบทอดมาจากการตรวจสอบรวม</span><span class="sxs-lookup"><span data-stu-id="8f1f7-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8f1f7-115">นี่เป็นหลักหมายความว่ารายงานการตรวจสอบแบบดั้งเดิมของทั้งหมดของทั้งหมดจะถูกขับเคลื่อนผ่านด้านหน้าและมีการโยกย้ายสัญญาณการตรวจสอบเดิม</span><span class="sxs-lookup"><span data-stu-id="8f1f7-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8f1f7-116">การเปลี่ยนแปลงที่สำคัญ:</span><span class="sxs-lookup"><span data-stu-id="8f1f7-116">Key changes:</span></span>

- <span data-ttu-id="8f1f7-117">การตัดแต่งเป็นความสามารถไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8f1f7-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="8f1f7-118">ส่วนที่คุณเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบจะไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8f1f7-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="8f1f7-119">โปรดดูที่[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สำหรับรายการทั้งหมดของเหตุการณ์ที่ตรวจสอบพร้อมใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="8f1f7-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="8f1f7-120">ตัวเลือก "ตำแหน่ง" ภายใต้**รายงานที่กำหนดเอง**ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8f1f7-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="8f1f7-121">เหตุการณ์ "การเปิดหรือดาวน์โหลดเอกสาร" ไม่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8f1f7-121">“Opening or downloading documents” events is NOT available.</span></span> 

