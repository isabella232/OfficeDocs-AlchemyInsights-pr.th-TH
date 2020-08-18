---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786908"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="f4dc1-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="f4dc1-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="f4dc1-103">การทำงานกับ PowerShell หรือสคริปต์ภายใน Sharepoint Online หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f4dc1-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="f4dc1-104">ไปที่ลิงก์ทางด้านล่างเพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f4dc1-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="f4dc1-105">การเริ่มต้นใช้งาน SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="f4dc1-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="f4dc1-106">เชื่อมต่อกับ SPO PowerShell ที่มีการรับรองความถูกต้องรับรอง (MFA)</span><span class="sxs-lookup"><span data-stu-id="f4dc1-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="f4dc1-107">[รูปแบบและหลักปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) มีไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการการจัดการที่ซับซ้อนต่อ SPO</span><span class="sxs-lookup"><span data-stu-id="f4dc1-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="f4dc1-108">ถ้าคุณกำลังมีปัญหาในการเชื่อมต่อกับ SPO management shell ตรวจสอบให้แน่ใจว่าคุณได้อัปเดตเป็นเวอร์ชันล่าสุดแล้วลอง [นำเข้าโมดูลใหม่](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) โดยใช้ *"นำเข้าโมดูลของไมโครซอฟท์ออนไลน์. PowerShell"*</span><span class="sxs-lookup"><span data-stu-id="f4dc1-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="f4dc1-109">ถ้าคุณกำลังพยายามเรียกใช้สคริปต์รูปแบบวัตถุฝั่งไคลเอ็นต์คุณจำเป็นต้องมีการติดตั้ง [SDK คอมโพเนนต์ของไคลเอ็นต์ Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) ไว้บนเครื่องภายในเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="f4dc1-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="f4dc1-110">ถ้าคุณกำลังมีปัญหาในการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาเรียกใช้ PowerShell ในฐานะผู้ดูแลระบบและการเปลี่ยนแปลง [นโยบายการดำเนิน](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)การ</span><span class="sxs-lookup"><span data-stu-id="f4dc1-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>