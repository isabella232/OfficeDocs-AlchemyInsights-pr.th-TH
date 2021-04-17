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
# <a name="troubleshooting-pst-import-issues"></a>การแก้ไขปัญหาการนําเข้า PST

- ถ้าคุณนําเข้าภายในไคลเอ็นต์ Outlook เอง โปรดดู[แก้ไขปัญหาการนําเข้าไฟล์ .pst ของ Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- ถ้าคุณใช้บริการการนําเข้าและค้าง โปรดทราบว่าไฟล์ PST แต่ละไฟล์ที่คุณอัปโหลดไปยังที่เก็บข้อมูล Azure ควรมีขนาดไม่เกิน 20 GB ไฟล์ PST ที่มีขนาดใหญ่กว่า 20 GB อาจส่งผลต่อประสิทธิภาพของกระบวนการนําเข้า PST

- ถ้าคุณต้องการตรวจสอบสถานะงานนําเข้าเฉพาะ คุณสามารถใช้ [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)ได้

- For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
