---
title: การแก้ไขปัญหาการนําเข้า PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991385"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="9ef9a-102">การแก้ไขปัญหาการนําเข้า PST</span><span class="sxs-lookup"><span data-stu-id="9ef9a-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="9ef9a-103">ถ้าคุณกําลังนําเข้าภายในไคลเอนต์ Outlook เอง โปรดดู[แก้ไขปัญหาการนําเข้าแฟ้ม.pst ของ Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="9ef9a-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="9ef9a-104">ถ้าคุณกําลังใช้บริการนําเข้า และติด โปรดทราบว่า แต่ละแฟ้ม PST ที่คุณอัปโหลดไปยังตําแหน่งที่เก็บ Azure ควรจะไม่มีขนาดใหญ่กว่า 20 กิกะไบต์</span><span class="sxs-lookup"><span data-stu-id="9ef9a-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="9ef9a-105">ไฟล์ PST มีขนาดใหญ่กว่า 20 GB อาจส่งผลกระทบต่อประสิทธิภาพของกระบวนการนําเข้า PST.</span><span class="sxs-lookup"><span data-stu-id="9ef9a-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="9ef9a-106">ถ้าคุณต้องการตรวจสอบสถานะของงานนําเข้าเฉพาะ[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)</span><span class="sxs-lookup"><span data-stu-id="9ef9a-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="9ef9a-107">สําหรับรายละเอียดทั้งหมดเกี่ยวกับบริการนําเข้า โปรดดู[ภาพรวมของการนําเข้าไฟล์ PST ขององค์กร](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9ef9a-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
