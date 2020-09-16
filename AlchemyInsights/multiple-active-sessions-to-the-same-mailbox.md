---
title: เซสชันที่ใช้งานอยู่หลายเซสชันไปยังกล่องจดหมายเดียวกัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769743"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="efd33-102">เซสชันที่ใช้งานอยู่หลายเซสชันไปยังกล่องจดหมายเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="efd33-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="efd33-103">เมื่อต้องการควบคุมการใช้ทรัพยากร Exchange กล่องจดหมายจะมี "งบประมาณ"</span><span class="sxs-lookup"><span data-stu-id="efd33-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="efd33-104">ข้อยกเว้นงบประมาณสามารถทริกเกอร์ได้แต่ไม่จำกัดเฉพาะสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="efd33-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="efd33-105">แท็บเบราว์เซอร์สองสามแท็บจะถูกเปิดภายในเซสชัน Outlook Web App เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="efd33-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="efd33-106">เซสชัน Outlook Web App ที่ใช้งานอยู่ไม่กี่รายการไปยังกล่องจดหมายเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="efd33-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="efd33-107">แอปพลิเคชันไคลเอ็นต์อื่นๆ (Outlook, Outlook Mobile, แอปไคลเอ็นต์ของบริษัทอื่น) เข้าถึงกล่องจดหมายในเวลาเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="efd33-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="efd33-108">การดำเนินการที่ใช้งานได้ยาวนานเช่นการดำเนินการคำขอการค้นหาจะดำเนินการจากเซสชันของกล่องจดหมายที่ใช้งานอยู่อื่น</span><span class="sxs-lookup"><span data-stu-id="efd33-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

