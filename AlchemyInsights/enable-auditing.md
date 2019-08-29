---
title: เปิดใช้งานและค้นหาบันทึกการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 9c8f38e7bfac6d5ac6f82e5d8225c89530bd98b2
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665095"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="46915-102">เปิดใช้งานและค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="46915-102">Enable and search the Audit log</span></span>

<span data-ttu-id="46915-103">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="46915-103">**Office 365**</span></span>

<span data-ttu-id="46915-104">หากต้องการค้นหาบันทึกการตรวจสอบ Office ๓๖๕ให้ทำตาม[ขั้นตอนเหล่านี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="46915-104">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="46915-105">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="46915-105">**Exchange**</span></span>

- <span data-ttu-id="46915-106">กิจกรรมการดูแลอัตราแลกเปลี่ยนจะถูกตรวจสอบโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="46915-106">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="46915-107">การตรวจสอบกล่องจดหมายถูกเปิดใช้งานโดยค่าเริ่มต้นใน Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="46915-107">Mailbox auditing is enabled by default in Office 365.</span></span> <span data-ttu-id="46915-108">สำหรับข้อมูลเพิ่มเติมโปรดดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="46915-108">For more information, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="46915-109">กล่องจดหมายของ Office ๓๖๕กลุ่มและกล่องจดหมายโฟลเดอร์สาธารณะใน Exchange แบบออนไลน์ไม่สนับสนุนการบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="46915-109">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="46915-110">**SharePoint และ OneDrive**</span><span class="sxs-lookup"><span data-stu-id="46915-110">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="46915-111">ไม่มีการกำหนดค่าเพิ่มเติมที่จำเป็นในการเปิดใช้งานการตรวจสอบสำหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="46915-111">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="46915-112">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="46915-112">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="46915-113">แฟ้มโฟลเดอร์และกิจกรรมเพจ</span><span class="sxs-lookup"><span data-stu-id="46915-113">File, folder, and page activities</span></span>
    - <span data-ttu-id="46915-114">การแชร์และการเข้าถึงกิจกรรมการร้องขอ</span><span class="sxs-lookup"><span data-stu-id="46915-114">Sharing and access request activities</span></span>
    - <span data-ttu-id="46915-115">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="46915-115">Site administration activities</span></span>
    - <span data-ttu-id="46915-116">กิจกรรมการซิงโครไนส์แฟ้ม</span><span class="sxs-lookup"><span data-stu-id="46915-116">File synchronization activities</span></span>

- <span data-ttu-id="46915-117">สำหรับข้อมูลเกี่ยวกับกิจกรรมที่ตรวจสอบในบริการ Office ๓๖๕อื่นๆโปรดดู[ตารางในบทความนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="46915-117">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="46915-118">ที่นี่รายการคำถามที่ถามบ่อยเกี่ยวกับคำถามที่[พบบ่อย](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions)เกี่ยวกับการค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="46915-118">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>