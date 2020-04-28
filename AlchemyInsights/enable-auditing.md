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
ms.openlocfilehash: 858228acdd884257fc68ceb99799a08e9cc0a0f8
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908435"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="58abb-102">เปิดใช้งานและค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="58abb-102">Enable and search the Audit log</span></span>

<span data-ttu-id="58abb-103">**ไมโครซอฟท์ 365**</span><span class="sxs-lookup"><span data-stu-id="58abb-103">**Microsoft 365**</span></span>

<span data-ttu-id="58abb-104">เมื่อต้องการค้นหาบันทึกการตรวจสอบ Microsoft 365 ให้ทําตามขั้นตอน[เหล่านี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="58abb-104">To search the Microsoft 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="58abb-105">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="58abb-105">**Exchange**</span></span>

- <span data-ttu-id="58abb-106">กิจกรรมการดูแลระบบ Exchange จะถูกตรวจสอบโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="58abb-106">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="58abb-107">กล่องจดหมายการตรวจสอบจะเปิดใช้งาน โดยค่าเริ่มต้นใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="58abb-107">Mailbox auditing is enabled by default in Microsoft 365.</span></span> <span data-ttu-id="58abb-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="58abb-108">For more information, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="58abb-109">กล่องจดหมายของกลุ่ม Microsoft 365 และกล่องจดหมายของโฟลเดอร์สาธารณะในการแลกเปลี่ยนแบบออนไลน์ไม่สนับสนุนการบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="58abb-109">Microsoft 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="58abb-110">**แชร์พอยท์และวันไดรฟ์**</span><span class="sxs-lookup"><span data-stu-id="58abb-110">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="58abb-111">ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นเพื่อเปิดใช้งานการตรวจสอบสําหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="58abb-111">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="58abb-112">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="58abb-112">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="58abb-113">แฟ้ม โฟลเดอร์ และกิจกรรมหน้า</span><span class="sxs-lookup"><span data-stu-id="58abb-113">File, folder, and page activities</span></span>
    - <span data-ttu-id="58abb-114">กิจกรรมการแชร์และการร้องขอการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="58abb-114">Sharing and access request activities</span></span>
    - <span data-ttu-id="58abb-115">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="58abb-115">Site administration activities</span></span>
    - <span data-ttu-id="58abb-116">กิจกรรมการซิงโครไนซ์ไฟล์</span><span class="sxs-lookup"><span data-stu-id="58abb-116">File synchronization activities</span></span>

- <span data-ttu-id="58abb-117">สําหรับข้อมูลเกี่ยวกับกิจกรรมที่ตรวจสอบแล้วในบริการอื่นๆ ให้ดูที่[ตารางใน บทความนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="58abb-117">For information about audited activities in other services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="58abb-118">ต่อไปนี้เป็นรายการ[คําถามที่ถามบ่อยเกี่ยวกับการค้นหา](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions)บันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="58abb-118">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>