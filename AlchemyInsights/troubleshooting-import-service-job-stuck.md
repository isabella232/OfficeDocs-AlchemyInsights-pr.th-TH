---
title: การแก้ไขปัญหาการนําเข้างานบริการค้าง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125496"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="13b4f-102">การแก้ไขปัญหาการนําเข้างานบริการค้าง</span><span class="sxs-lookup"><span data-stu-id="13b4f-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="13b4f-103">ถ้าคุณพบปัญหาเกี่ยวกับการนําเข้างานบริการค้างหรือล้มเหลว ให้ตรวจสอบและลองใช้วิธีต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="13b4f-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="13b4f-104">ตรวจสอบขนาดของไฟล์ PST</span><span class="sxs-lookup"><span data-stu-id="13b4f-104">Review the size of of the PST file.</span></span> <span data-ttu-id="13b4f-105">ขนาดสูงสุดที่แนะนําของไฟล์ PST เพื่อนําเข้าคือ 20 GB</span><span class="sxs-lookup"><span data-stu-id="13b4f-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="13b4f-106">ถ้าคุณสงสัยรายการที่ข้ามเนื่องจากความเสียหาย ให้เรียกใช้Scanpst.exeวินิจฉัยและแก้ไขข้อผิดพลาดในไฟล์ PST</span><span class="sxs-lookup"><span data-stu-id="13b4f-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="13b4f-107">ถ้าคุณเห็นข้อผิดพลาด "MapiExceptionShutoffQuotaExceeded" ระหว่างการนําเข้า ให้ตรวจสอบให้แน่ใจว่ากล่องจดหมายเป้าหมายมีความจุเพียงพอที่จะนําเข้าไฟล์ PST ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="13b4f-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="13b4f-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="13b4f-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="13b4f-109">For information about how to fix issues when importing PSTs into Outlook, [see Fix problems importing an Outlook .pst (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="13b4f-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>