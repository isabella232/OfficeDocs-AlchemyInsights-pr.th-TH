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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972438"
---
# <a name="troubleshooting-pst-import-issues"></a>การแก้ไขปัญหาการนําเข้า PST

- ถ้าคุณนําเข้าภายในไคลเอ็นต์ Outlook ให้ดูที่[แก้ไขปัญหาการนําเข้าOutlookไฟล์ .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- ถ้าคุณใช้บริการการนําเข้าและค้างอยู่ โปรดทราบว่าไฟล์ PST แต่ละไฟล์ที่คุณอัปโหลดไปยังที่เก็บข้อมูล Azure ควรมีขนาดไม่เกิน 20GB ไฟล์ PST ที่มีขนาดใหญ่กว่า 20 GB อาจส่งผลต่อประสิทธิภาพการนําเข้าของกระบวนการนําเข้า PST For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- ถ้าคุณต้องการตรวจสอบสถานะงานนําเข้าเฉพาะ ให้ใช้[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
