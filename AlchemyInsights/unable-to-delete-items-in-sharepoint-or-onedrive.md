---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049536"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการได้

มีปัญหาในการลบรายการ SharePoint หรือไม่

- โปรดตรวจสอบให้แน่ใจว่าคุณมี[สิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)เพื่อลบรายการหรือมี[ผู้ดูแลชุดเก็บรวบรวมไซต์](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)พยายามเอารายการออก

- ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies)ในสินค้า

- ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น

- ในที่สุดผู้ดูแลระบบสามารถใช้[รูปแบบและวิธีปฏิบัติของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการจัดการที่ซับซ้อนเช่นการบังคับให้ลบรายการที่ปากแข็ง
- [เอาแฟ้ม PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [ลบโฟลเดอร์ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [ลบรายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [ลบรายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [ลบฟิลด์ PNP (คอลัมน์)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)