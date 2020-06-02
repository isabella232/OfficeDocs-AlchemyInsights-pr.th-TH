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
ms.openlocfilehash: d6f1f96220a44247d217f6e82e76fb38875578e8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507009"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="f3c15-102">เปิดใช้งานและค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="f3c15-102">Enable and search the Audit log</span></span>

<span data-ttu-id="f3c15-103">**ไมโครซอฟท์ 365**</span><span class="sxs-lookup"><span data-stu-id="f3c15-103">**Microsoft 365**</span></span>

<span data-ttu-id="f3c15-104">เมื่อต้องการค้นหาบันทึกการตรวจสอบ Microsoft 365 ให้ทําตามขั้นตอน[เหล่านี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="f3c15-104">To search the Microsoft 365 audit log, follow [these steps](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="f3c15-105">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="f3c15-105">**Exchange**</span></span>

- <span data-ttu-id="f3c15-106">กิจกรรมของผู้ดูแลระบบ Exchange จะถูกตรวจสอบโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f3c15-106">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="f3c15-107">การตรวจสอบกล่องจดหมายถูกเปิดใช้งาน โดยค่าเริ่มต้นใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f3c15-107">Mailbox auditing is enabled by default in Microsoft 365.</span></span> <span data-ttu-id="f3c15-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="f3c15-108">For more information, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="f3c15-109">กล่องจดหมายของ Microsoft 365 กลุ่มและกล่องจดหมายของโฟลเดอร์สาธารณะในการแลกเปลี่ยนแบบออนไลน์ไม่สนับสนุนการบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="f3c15-109">Microsoft 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="f3c15-110">**1000000000000000**</span><span class="sxs-lookup"><span data-stu-id="f3c15-110">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="f3c15-111">ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นเพื่อเปิดใช้งานการตรวจสอบสําหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="f3c15-111">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="f3c15-112">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f3c15-112">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="f3c15-113">โฟลเดอร์ และกิจกรรมของเพจ</span><span class="sxs-lookup"><span data-stu-id="f3c15-113">File, folder, and page activities</span></span>
    - <span data-ttu-id="f3c15-114">การแชร์และการเข้าถึงกิจกรรมคําขอ</span><span class="sxs-lookup"><span data-stu-id="f3c15-114">Sharing and access request activities</span></span>
    - <span data-ttu-id="f3c15-115">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="f3c15-115">Site administration activities</span></span>
    - <span data-ttu-id="f3c15-116">กิจกรรมการทําข้อมูลแฟ้มให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="f3c15-116">File synchronization activities</span></span>

- <span data-ttu-id="f3c15-117">สําหรับข้อมูลเกี่ยวกับกิจกรรมที่ตรวจสอบในบริการอื่นๆ ให้ดู[ตารางในบทความนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="f3c15-117">For information about audited activities in other services, see  [the table in this article](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="f3c15-118">นี่คือรายการ[คําถามที่ถามบ่อยเกี่ยวกับการค้นหา](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions)บันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="f3c15-118">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>