---
title: บันทึกการตรวจสอบเปิดใช้งานและการค้นหา
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 8c965cb1c2b6a4cb46b5c1b0145932c4c54ba97d
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270547"
---
# <a name="enable-and-search-audit-log"></a><span data-ttu-id="cb5c1-102">บันทึกการตรวจสอบเปิดใช้งานและการค้นหา</span><span class="sxs-lookup"><span data-stu-id="cb5c1-102">Enable and search Audit log</span></span>

<span data-ttu-id="cb5c1-103">เมื่อต้องการค้นหาบันทึกการตรวจสอบ Office 365 ให้ทำตาม[ขั้นตอนเหล่านี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="cb5c1-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="cb5c1-104">**อัตราแลกเปลี่ยน**</span><span class="sxs-lookup"><span data-stu-id="cb5c1-104">**Exchange**</span></span>

- <span data-ttu-id="cb5c1-105">แลกเปลี่ยน admin กิจกรรมจะได้รับการตรวจสอบ โดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="cb5c1-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="cb5c1-106">เรากำลังอยู่ในระหว่างการเปิดใช้งานการตรวจสอบจดหมาย โดยค่าเริ่มต้นใน Office 365</span><span class="sxs-lookup"><span data-stu-id="cb5c1-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="cb5c1-107">จนกว่านั้น เมื่อต้องการเปิดใช้งานการตรวจสอบ สำหรับกล่องจดหมายเดียว หรือ สำหรับกล่องจดหมายทั้งหมดในองค์กรของคุณ ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="cb5c1-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="cb5c1-108">กล่องจดหมายกลุ่ม office 365 และกล่องจดหมายโฟลเดอร์สาธารณะในการแลกเปลี่ยนแบบออนไลน์ไม่สนับสนุนการบันทึกข้อมูลการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="cb5c1-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="cb5c1-109">**SharePoint และ OneDrive**</span><span class="sxs-lookup"><span data-stu-id="cb5c1-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="cb5c1-110">ไม่มีการกำหนดค่าไม่มีเพิ่มเติมที่จำเป็นสำหรับการเปิดใช้งานการตรวจสอบสำหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="cb5c1-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="cb5c1-111">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="cb5c1-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="cb5c1-112">ไฟล์ โฟลเดอร์ และหน้ากิจกรรม</span><span class="sxs-lookup"><span data-stu-id="cb5c1-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="cb5c1-113">กิจกรรมการร้องขอการเข้าถึงและการใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="cb5c1-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="cb5c1-114">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="cb5c1-114">Site administration activities</span></span>
    - <span data-ttu-id="cb5c1-115">กิจกรรมที่ซิงโครไนส์ไฟล์</span><span class="sxs-lookup"><span data-stu-id="cb5c1-115">File synchronization activities</span></span>

- <span data-ttu-id="cb5c1-116">สำหรับข้อมูลเกี่ยวกับการตรวจสอบกิจกรรมในบริการ Office 365 อื่น ๆ ดู[ตารางในบทความนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="cb5c1-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="cb5c1-117">รายการของคำถามที่ถามบ่อย[คำถามที่ถามบ่อย](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions)เกี่ยวกับการค้นหาบันทึกการตรวจสอบที่นี่</span><span class="sxs-lookup"><span data-stu-id="cb5c1-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>