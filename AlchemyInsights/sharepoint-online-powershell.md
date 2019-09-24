---
title: PowerShell แบบออนไลน์ของ Sharepoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123017"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="1e7c8-102">PowerShell แบบออนไลน์ของ Sharepoint</span><span class="sxs-lookup"><span data-stu-id="1e7c8-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="1e7c8-103">การทำงานกับ PowerShell หรือสคริปต์ภายใน Sharepoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1e7c8-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="1e7c8-104">โปรดไปที่ลิงก์ด้านล่างเพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1e7c8-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="1e7c8-105">การเริ่มต้นใช้งานเชลล์จัดการออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="1e7c8-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="1e7c8-106">เชื่อมต่อกับการตรวจสอบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="1e7c8-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="1e7c8-107">[รูปแบบและวิธีปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)ประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการจัดการที่ซับซ้อนไปยังที่ได้</span><span class="sxs-lookup"><span data-stu-id="1e7c8-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="1e7c8-108">ถ้าคุณกำลังมีปัญหาในการเชื่อมต่อกับเชลล์จัดการใหม่ตรวจสอบให้แน่ใจว่าคุณได้ปรับปรุงเป็นรุ่นล่าสุดและพยายามที่จะ[นำเข้าโมดูล](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)โดยใช้ *"นำเข้าโมดูล Microsoft. PowerShell"*</span><span class="sxs-lookup"><span data-stu-id="1e7c8-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="1e7c8-109">ถ้าคุณกำลังพยายามเรียกใช้สคริปต์รูปแบบวัตถุฝั่งไคลเอ็นต์คุณจะต้องมี[SDK คอมโพเนนต์ของไคลเอ็นต์ Sharepoint แบบออนไลน์](https://www.microsoft.com/download/details.aspx?id=42038)ที่ติดตั้งบนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e7c8-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="1e7c8-110">ถ้าคุณกำลังมีปัญหาในการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาเรียกใช้ PowerShell ในฐานะผู้ดูแลและการเปลี่ยนแปลง[นโยบายการดำเนิน](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)การ</span><span class="sxs-lookup"><span data-stu-id="1e7c8-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>