---
title: การตรวจสอบใน Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430065"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="e4c91-102">การตรวจสอบใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e4c91-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="e4c91-103">ต่อไปนี้เป็นบางสิ่งที่คุณควรทราบเกี่ยวกับการตรวจสอบใน Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="e4c91-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="e4c91-104">กิจกรรมผู้ดูแลระบบ Exchange จะถูกตรวจสอบตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="e4c91-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="e4c91-105">เราอยู่ในระหว่างการเปิดใช้งานการตรวจสอบกล่องจดหมายตามค่าเริ่มต้นของผู้ใช้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e4c91-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="e4c91-106">เมื่อต้องการอ่านเพิ่มเติมเกี่ยวกับเรื่องนี้ [ให้คลิก](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)ที่นี่</span><span class="sxs-lookup"><span data-stu-id="e4c91-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="e4c91-107">จนกว่าจะถึงตอนนี้ ถ้าคุณต้องการคําแนะนําให้เปิดใช้งานด้วยตนเองให้กับบุคคลหนึ่งคนหรือทั้งองค์กร ให้เลือกปุ่มเปิดการตรวจสอบกล่องจดหมายด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="e4c91-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="e4c91-108">กล่องจดหมายกลุ่ม Microsoft 365 และกล่องจดหมายโฟลเดอร์สาธารณะไม่สนับสนุนบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="e4c91-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="e4c91-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span><span class="sxs-lookup"><span data-stu-id="e4c91-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="e4c91-110">เมื่อต้องการเรียนรู้ว่ากิจกรรมอะไรได้รับการตรวจสอบ ให้ดู:</span><span class="sxs-lookup"><span data-stu-id="e4c91-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="e4c91-111">กิจกรรมของไฟล์</span><span class="sxs-lookup"><span data-stu-id="e4c91-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="e4c91-112">กิจกรรมของโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="e4c91-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="e4c91-113">[กิจกรรมการแชร์และ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)การเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="e4c91-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="e4c91-114">ดูกิจกรรมผ่านการตรวจสอบทั้งหมดตามบริการ [จากรายการกิจกรรมที่ผ่าน](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)การตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="e4c91-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
