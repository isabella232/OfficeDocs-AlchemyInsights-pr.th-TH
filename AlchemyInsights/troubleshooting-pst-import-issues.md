---
title: การแก้ไขปัญหาการนำเข้า PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757759"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="399e3-102">การแก้ไขปัญหาการนำเข้า PST</span><span class="sxs-lookup"><span data-stu-id="399e3-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="399e3-103">ถ้าคุณกำลังนำเข้าภายในไคลเอ็นต์ Outlook เองโปรดดู[แก้ไขปัญหาการนำเข้าไฟล์ .pst ของ Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="399e3-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="399e3-104">ถ้าคุณกำลังใช้บริการนำเข้าและการติดตั้งโปรดทราบว่าแต่ละไฟล์ PST ที่คุณอัปโหลดไปยังตำแหน่งที่เก็บ Azure ควรจะมีขนาดใหญ่กว่า20กิกะไบต์</span><span class="sxs-lookup"><span data-stu-id="399e3-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="399e3-105">ไฟล์ PST ที่มีขนาดใหญ่กว่า 20 GB อาจส่งผลกระทบต่อประสิทธิภาพการทำงานของกระบวนการนำเข้า PST</span><span class="sxs-lookup"><span data-stu-id="399e3-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="399e3-106">ถ้าคุณต้องการตรวจสอบสถานะของงานนำเข้าที่เฉพาะเจาะจงคุณสามารถใช้ [MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)ได้</span><span class="sxs-lookup"><span data-stu-id="399e3-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="399e3-107">สำหรับรายละเอียดทั้งหมดเกี่ยวกับบริการนำเข้าโปรดดู[ภาพรวมของการนำเข้าไฟล์ PST ขององค์กรของคุณ](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="399e3-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
