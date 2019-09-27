---
title: ตำแหน่งของข้อมูล
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207280"
---
# <a name="data-location"></a><span data-ttu-id="70476-102">ตำแหน่งของข้อมูล</span><span class="sxs-lookup"><span data-stu-id="70476-102">Data location</span></span>

<span data-ttu-id="70476-103">คุณสามารถดูตำแหน่งที่ตั้งของผู้เช่า Office ๓๖๕ของคุณในศูนย์การจัดการหรือโดยการเชื่อมต่อกับ Exchange แบบออนไลน์ผ่านทาง PowerShell</span><span class="sxs-lookup"><span data-stu-id="70476-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="70476-104">**ศูนย์การจัดการ:**</span><span class="sxs-lookup"><span data-stu-id="70476-104">**Admin center:**</span></span>
1. <span data-ttu-id="70476-105">ล็อกอินเข้าสู่[ศูนย์กลางการดูแล](https://admin.microsoft.com/Adminportal/Home)ระบบ</span><span class="sxs-lookup"><span data-stu-id="70476-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="70476-106">เลือก**โปรไฟล์องค์กร\*\*\*\*การตั้งค่า** > </span><span class="sxs-lookup"><span data-stu-id="70476-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="70476-107">ภายใต้**ตำแหน่งข้อมูล**ให้เลือก**ดูรายละเอียด**</span><span class="sxs-lookup"><span data-stu-id="70476-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="70476-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="70476-108">**PowerShell:**</span></span>
1. <span data-ttu-id="70476-109">เชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์โดยใช้ Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="70476-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="70476-110">ดำเนินการ cmdlet การ[รับองค์กร](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit)เพื่อแสดงรายการของคุณสมบัติของผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="70476-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="70476-111">มองไปที่คุณสมบัติองค์กร</span><span class="sxs-lookup"><span data-stu-id="70476-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="70476-112">เมื่อคุณมีตำแหน่งข้อมูลสำหรับ EXO และที่คุณสามารถกำหนดตำแหน่งข้อมูลสำหรับบริการอื่นๆที่คุณอาจใช้จาก[ตำแหน่งที่ข้อมูลของคุณอยู่](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="70476-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>