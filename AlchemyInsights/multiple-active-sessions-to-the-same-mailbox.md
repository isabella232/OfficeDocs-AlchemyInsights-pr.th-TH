---
title: เซสชันที่ใช้งานอยู่หลายไปยังกล่องจดหมายเดียวกัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439723"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="808d3-102">เซสชันที่ใช้งานอยู่หลายไปยังกล่องจดหมายเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="808d3-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="808d3-103">เมื่อต้องการควบคุมการใช้ทรัพยากร Exchange กล่องจดหมายมี "งบประมาณ"</span><span class="sxs-lookup"><span data-stu-id="808d3-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="808d3-104">ข้อยกเว้นเกินงบประมาณสามารถเรียกโดย แต่ไม่ จํากัด เฉพาะสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="808d3-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="808d3-105">แท็บเบราว์เซอร์สองสามแท็บจะเปิดภายในเซสชัน Outlook Web App เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="808d3-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="808d3-106">เซสชัน Outlook Web App ที่ใช้งานเพียงไม่กี่เซสชันไปยังกล่องจดหมายเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="808d3-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="808d3-107">โปรแกรมประยุกต์ไคลเอนต์อื่น ๆ (Outlook, Outlook Mobile, แอปไคลเอ็นต์ของบุคคลที่สาม) เข้าถึงกล่องจดหมายในเวลาเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="808d3-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="808d3-108">การดําเนินการที่รันเป็นเวลานาน เช่น การดําเนินการร้องขอการค้นหา จะดําเนินการจากเซสชันกล่องจดหมายที่ใช้งานอยู่อื่น</span><span class="sxs-lookup"><span data-stu-id="808d3-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

