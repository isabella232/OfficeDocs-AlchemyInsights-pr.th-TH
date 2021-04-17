---
title: การแก้ไขปัญหาการนําเข้า PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826182"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="14fb3-102">การแก้ไขปัญหาการนําเข้า PST</span><span class="sxs-lookup"><span data-stu-id="14fb3-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="14fb3-103">ถ้าคุณนําเข้าภายในไคลเอ็นต์ Outlook เอง โปรดดู[แก้ไขปัญหาการนําเข้าไฟล์ .pst ของ Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="14fb3-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="14fb3-104">ถ้าคุณใช้บริการการนําเข้าและค้าง โปรดทราบว่าไฟล์ PST แต่ละไฟล์ที่คุณอัปโหลดไปยังที่เก็บข้อมูล Azure ควรมีขนาดไม่เกิน 20 GB</span><span class="sxs-lookup"><span data-stu-id="14fb3-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="14fb3-105">ไฟล์ PST ที่มีขนาดใหญ่กว่า 20 GB อาจส่งผลต่อประสิทธิภาพของกระบวนการนําเข้า PST</span><span class="sxs-lookup"><span data-stu-id="14fb3-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="14fb3-106">ถ้าคุณต้องการตรวจสอบสถานะงานนําเข้าเฉพาะ คุณสามารถใช้ [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)ได้</span><span class="sxs-lookup"><span data-stu-id="14fb3-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="14fb3-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="14fb3-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
