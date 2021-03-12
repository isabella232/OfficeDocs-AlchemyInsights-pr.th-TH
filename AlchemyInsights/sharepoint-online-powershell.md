---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709089"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="1efbb-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="1efbb-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="1efbb-103">ต้องการใช้งาน PowerShell หรือสคริปต์ภายใน Sharepoint Online ใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="1efbb-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="1efbb-104">ไปที่ลิงก์ด้านล่างเพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1efbb-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="1efbb-105">เริ่มต้นใช้งาน SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="1efbb-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="1efbb-106">เชื่อมต่อกับ SPO PowerShell ที่มีการรับรองความถูกต้องแบบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="1efbb-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="1efbb-107">[รูปแบบและหลักปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) มีไลบรารีของสั่ง PowerShell ที่ช่วยให้คุณสามารถจัดการที่ซับซ้อนต่อ SPO ได้</span><span class="sxs-lookup"><span data-stu-id="1efbb-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="1efbb-108">ถ้าคุณมีปัญหาในการเชื่อมต่อกับเชลล์การจัดการ SPO ตรวจสอบให้แน่ใจว่าคุณได้อัปเดตเป็นเวอร์ชันล่าสุดแล้วและพยายามนําเข้ามอดูลอีกครั้งโดยใช้ *"Import-Module Microsoft.Online.SharePoint.PowerShell"* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)</span><span class="sxs-lookup"><span data-stu-id="1efbb-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="1efbb-109">ถ้าคุณพยายามเรียกใช้สคริปต์โมเดลวัตถุที่ฝั่งไคลเอ็นต์ คุณจะต้องติดตั้ง [SharePoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) บนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="1efbb-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="1efbb-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="1efbb-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>