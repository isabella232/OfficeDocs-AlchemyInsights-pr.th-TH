---
title: ตําแหน่งที่ตั้งข้อมูล
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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655301"
---
# <a name="data-location"></a><span data-ttu-id="2443c-102">ตําแหน่งที่ตั้งข้อมูล</span><span class="sxs-lookup"><span data-stu-id="2443c-102">Data location</span></span>

<span data-ttu-id="2443c-103">คุณสามารถดูตําแหน่งที่ตั้งของผู้เช่าของคุณในศูนย์การจัดการ หรือโดยการเชื่อมต่อกับ Exchange Online ผ่านทาง PowerShell</span><span class="sxs-lookup"><span data-stu-id="2443c-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="2443c-104">**ศูนย์การจัดการ:**</span><span class="sxs-lookup"><span data-stu-id="2443c-104">**Admin center:**</span></span>
1. <span data-ttu-id="2443c-105">เข้าสู่ระบบ[ที่ ศูนย์การจัดการ](https://admin.microsoft.com/Adminportal/Home)</span><span class="sxs-lookup"><span data-stu-id="2443c-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="2443c-106">เลือก**โปรไฟล์องค์กร\*\*\*\*การตั้งค่า** > </span><span class="sxs-lookup"><span data-stu-id="2443c-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="2443c-107">ภายใต้**ตําแหน่งที่ตั้งข้อมูล\*\*\*\*ให้เลือก**</span><span class="sxs-lookup"><span data-stu-id="2443c-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="2443c-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="2443c-108">**PowerShell:**</span></span>
1. <span data-ttu-id="2443c-109">เชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์ โดยใช้ Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="2443c-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="2443c-110">ดําเนินการ cmdlet[รับ OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit)เพื่อแสดงรายการของคุณสมบัติของผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="2443c-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="2443c-111">ดูที่คุณสมบัติรหัสองค์กร</span><span class="sxs-lookup"><span data-stu-id="2443c-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="2443c-112">เมื่อคุณมีตําแหน่งข้อมูลสําหรับ EXO และ SPO คุณสามารถกําหนดตําแหน่งข้อมูลสําหรับบริการอื่น ๆ ที่คุณอาจใช้จาก[ตําแหน่งข้อมูลของคุณอยู่](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="2443c-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>