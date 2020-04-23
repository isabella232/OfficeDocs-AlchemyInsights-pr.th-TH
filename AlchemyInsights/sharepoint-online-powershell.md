---
title: พาวเวอร์เชลล์ออนไลน์ของ SharePoint
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764282"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="3f6c0-102">พาวเวอร์เชลล์ออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="3f6c0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="3f6c0-103">การทํางานกับ PowerShell หรือสคริปต์ภายใน Sharepoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="3f6c0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="3f6c0-104">ไปที่ลิงค์ด้านล่างสําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3f6c0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="3f6c0-105">การเริ่มต้นใช้งานเชลล์การจัดการแบบออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="3f6c0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="3f6c0-106">เชื่อมต่อกับ SPO PowerShell ด้วยการตรวจสอบสิทธิ์แบบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="3f6c0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="3f6c0-107">[รูปแบบและแนวปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)ประกอบด้วยไลบรารีของคําสั่ง PowerShell ที่ช่วยให้คุณสามารถดําเนินการจัดการที่ซับซ้อนต่อ SPO</span><span class="sxs-lookup"><span data-stu-id="3f6c0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="3f6c0-108">ถ้าคุณกําลังมีปัญหาในการเชื่อมต่อกับเชลล์การจัดการ SPO โปรดตรวจสอบให้แน่ใจว่า คุณได้ปรับปรุงเป็นรุ่นล่าสุด และลอง[นําเข้าโมดูล](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)โดยใช้ *"นําเข้าโมดูล Microsoft.SharePoint.SharePoint.PowerShell"* อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="3f6c0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="3f6c0-109">ถ้าคุณกําลังพยายามเรียกใช้สคริปต์ของวัตถุฝั่งไคลเอ็นต์แบบจําลอง คุณจะต้องมี[SDK คอมโพเนนต์ของไคลเอ็นต์ออนไลน์ของ Sharepoint](https://www.microsoft.com/download/details.aspx?id=42038)ที่ติดตั้งบนเครื่องของคุณภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="3f6c0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="3f6c0-110">ถ้าคุณมีปัญหาการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาการเรียกใช้ PowerShell เป็นผู้ดูแลระบบ และการเปลี่ยนแปลง[นโยบายการดําเนินการ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="3f6c0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>