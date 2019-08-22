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
ms.openlocfilehash: dea8f2ab0f99e493d68aa074532f26f7ed8026aa
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504410"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="d0220-102">SharePoint และ OneDrive แฟ้มบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="d0220-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="d0220-103">**ล็อก SharePoint และตรวจสอบที่รวมสมัยใหม่ OneDrive จากการปฏิบัติตามกฎระเบียบ**</span><span class="sxs-lookup"><span data-stu-id="d0220-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="d0220-104">เปิด/ปิดการเข้าสู่ ระบบตรวจสอบรวม</span><span class="sxs-lookup"><span data-stu-id="d0220-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="d0220-105">ไม่มีการตั้งค่าคอนฟิกเพิ่มเติมที่ถูกต้องภายใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="d0220-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="d0220-106">ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ โฟลเดอร์ ผู้ใช้ สิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="d0220-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="d0220-107">แฟ้มและหน้ากิจกรรม</span><span class="sxs-lookup"><span data-stu-id="d0220-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="d0220-108">กิจกรรมของโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="d0220-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="d0220-109">กิจกรรมการร้องขอการเข้าถึงและการใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="d0220-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="d0220-110">ซิงโครไนส์กิจกรรม</span><span class="sxs-lookup"><span data-stu-id="d0220-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="d0220-111">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="d0220-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="d0220-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการรับเหตุการณ์เหล่านี้ ดู[บันทึกการตรวจสอบการค้นหา](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="d0220-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="d0220-113">**ล็อกการตรวจสอบแบบคลาสสิกของ SharePoint**</span><span class="sxs-lookup"><span data-stu-id="d0220-113">**SharePoint classic Audit logs**</span></span>

- [<span data-ttu-id="d0220-114">ดู และเปิดใช้งานการบันทึกการตรวจสอบของ SharePoint แบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="d0220-114">View and enable classic SharePoint Audit logs</span></span>](https://support.office.com/article/view-audit-log-reports-b37c5869-1b47-4a82-a30d-ea20070fe527)

<span data-ttu-id="d0220-115">จำเป็นต้องตรวจสอบการเปิดใช้งานสำหรับแต่ละไซต์คอลเลกชันแต่ละ</span><span class="sxs-lookup"><span data-stu-id="d0220-115">Auditing need to be enabled per each site collection.</span></span> 

<span data-ttu-id="d0220-116">**หมายเหตุ**: เราขอแนะนำให้ใช้แบบสมัยใหม่รวมการตรวจสอบแฟ้มบันทึกสำหรับตัวเลือกการตรวจสอบขั้นสูง และดีกว่าบันทึกการตรวจสอบแบบคลาสสิกเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="d0220-116">**Note**: We recommend using Modern Unified Audit logs for better and advanced audit options than these classic audit logs.</span></span>

