---
title: เปิดใช้งานและค้นหาบันทึกการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a28e1f5bb8b5e1bff2f26c0d9e9c9c42e8324583
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806598"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="87338-102">เปิดใช้งานและค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="87338-102">Enable and search the Audit log</span></span>

<span data-ttu-id="87338-103">**Microsoft ๓๖๕**</span><span class="sxs-lookup"><span data-stu-id="87338-103">**Microsoft 365**</span></span>

<span data-ttu-id="87338-104">เมื่อต้องการค้นหาบันทึกการตรวจสอบของ Microsoft ๓๖๕ให้ทำตาม[ขั้นตอนต่อไปนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="87338-104">To search the Microsoft 365 audit log, follow [these steps](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="87338-105">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="87338-105">**Exchange**</span></span>

- <span data-ttu-id="87338-106">กิจกรรมผู้ดูแลระบบ Exchange จะถูกตรวจสอบตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="87338-106">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="87338-107">การตรวจสอบกล่องจดหมายจะถูกเปิดใช้งานตามค่าเริ่มต้นใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="87338-107">Mailbox auditing is enabled by default in Microsoft 365.</span></span> <span data-ttu-id="87338-108">สำหรับข้อมูลเพิ่มเติมให้ดู[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="87338-108">For more information, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="87338-109">กล่องจดหมายของกลุ่ม Microsoft ๓๖๕และกล่องจดหมายโฟลเดอร์สาธารณะใน Exchange Online ไม่สนับสนุนการบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="87338-109">Microsoft 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="87338-110">**SharePoint และ OneDrive**</span><span class="sxs-lookup"><span data-stu-id="87338-110">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="87338-111">ไม่มีการกำหนดค่าเพิ่มเติมที่จำเป็นสำหรับการเปิดใช้งานการตรวจสอบสำหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="87338-111">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="87338-112">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="87338-112">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="87338-113">ไฟล์โฟลเดอร์และกิจกรรมของหน้า</span><span class="sxs-lookup"><span data-stu-id="87338-113">File, folder, and page activities</span></span>
    - <span data-ttu-id="87338-114">การแชร์และการร้องขอการเข้าถึงกิจกรรม</span><span class="sxs-lookup"><span data-stu-id="87338-114">Sharing and access request activities</span></span>
    - <span data-ttu-id="87338-115">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="87338-115">Site administration activities</span></span>
    - <span data-ttu-id="87338-116">กิจกรรมการซิงโครไนซ์ไฟล์</span><span class="sxs-lookup"><span data-stu-id="87338-116">File synchronization activities</span></span>

- <span data-ttu-id="87338-117">สำหรับข้อมูลเกี่ยวกับกิจกรรมที่ตรวจสอบแล้วในบริการอื่นๆให้ดู[ที่ตารางในบทความนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="87338-117">For information about audited activities in other services, see  [the table in this article](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="87338-118">นี่คือรายการคำถามที่ถามบ่อยเกี่ยวกับคำถามที่ถาม [บ่อยเกี่ยวกับการ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) ค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="87338-118">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>