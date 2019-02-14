---
title: 286-เปิดใช้งานการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 59634675d859280fdef8ea476ff5a739e0684b86
ms.sourcegitcommit: 6bd248764239282688cac98347c2356b701389e4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982155"
---
# <a name="search-the-audit-log"></a><span data-ttu-id="ab399-102">ค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="ab399-102">Search the audit log</span></span>

<span data-ttu-id="ab399-103">เมื่อต้องการค้นหาบันทึกการตรวจสอบ Office 365 ให้ทำตาม[ขั้นตอนเหล่านี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="ab399-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span> 

<span data-ttu-id="ab399-104">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="ab399-104">**Exchange**</span></span>

- <span data-ttu-id="ab399-105">แลกเปลี่ยน admin กิจกรรมจะได้รับการตรวจสอบ โดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="ab399-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="ab399-p101">เรากำลังอยู่ในระหว่างการเปิดใช้งานการตรวจสอบจดหมาย โดยค่าเริ่มต้นใน Office 365 จนกว่านั้น เมื่อต้องการเปิดใช้งานการตรวจสอบ สำหรับกล่องจดหมายเดียว หรือ สำหรับกล่องจดหมายทั้งหมดในองค์กรของคุณ ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)</span><span class="sxs-lookup"><span data-stu-id="ab399-p101">We are in the process of enabling mailbox auditing by default in Office 365. Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="ab399-108">กล่องจดหมายกลุ่ม office 365 และกล่องจดหมายโฟลเดอร์สาธารณะในการแลกเปลี่ยนแบบออนไลน์ไม่สนับสนุนการบันทึกข้อมูลการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="ab399-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="ab399-109">**SharePoint และ OneDrive**</span><span class="sxs-lookup"><span data-stu-id="ab399-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="ab399-110">ไม่มีการกำหนดค่าไม่มีเพิ่มเติมที่จำเป็นสำหรับการเปิดใช้งานการตรวจสอบสำหรับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="ab399-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="ab399-111">SharePoint และ OneDrive สนับสนุนการตรวจสอบชนิดของกิจกรรมต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ab399-111">SharePoint and OneDrive support auditing the following types of activities:</span></span> 

    - <span data-ttu-id="ab399-112">ไฟล์ โฟลเดอร์ และหน้ากิจกรรม</span><span class="sxs-lookup"><span data-stu-id="ab399-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="ab399-113">กิจกรรมการร้องขอการเข้าถึงและการใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="ab399-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="ab399-114">กิจกรรมการดูแลไซต์</span><span class="sxs-lookup"><span data-stu-id="ab399-114">Site administration activities</span></span>
    - <span data-ttu-id="ab399-115">กิจกรรมที่ซิงโครไนส์ไฟล์</span><span class="sxs-lookup"><span data-stu-id="ab399-115">File synchronization activities</span></span>

- <span data-ttu-id="ab399-116">สำหรับข้อมูลเกี่ยวกับการตรวจสอบกิจกรรมในบริการ Office 365 อื่น ๆ ดู[ตารางในบทความนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="ab399-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="ab399-117">รายการของคำถามที่ถามบ่อย[คำถามที่ถามบ่อย](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions)เกี่ยวกับการค้นหาบันทึกการตรวจสอบที่นี่</span><span class="sxs-lookup"><span data-stu-id="ab399-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>