---
title: ไม่สามารถลบสินค้าใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057788"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการ

มีปัญหาการลบรายการหรือไม่

- เสมอให้แน่ใจว่า คุณมี[สิทธิ์ที่เหมาะสม](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups)เพื่อลบรายการ หรือมีความพยายามของ[ผู้ดูแลชุดเก็บรวบรวมไซต์](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)เอารายการนี้ออก

- ให้แน่ใจว่า ไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies)บนสินค้า

- ให้แน่ใจว่า สินค้าจะไม่[ถูกเช็คเอาท์](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น

- ในตอนท้าย ผู้ดูแลระบบสามารถใช้[รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) ซึ่งประกอบด้วยไลบรารีของ PowerShell คำสั่งที่อนุญาตให้คุณทำการดำเนินการจัดการที่ซับซ้อนเช่น บังคับให้ลบรายการ stubborn 
- [ลบไฟล์ PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [เอาโฟลเดอร์ PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [ลบสินค้าในรายการ PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [เอารายการ PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [เอา PNP เขตข้อมูล (คอลัมน์)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)