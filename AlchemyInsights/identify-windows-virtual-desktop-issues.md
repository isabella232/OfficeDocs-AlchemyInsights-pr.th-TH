---
title: ระบุปัญหาเดสก์ท็อปเสมือนของ Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596036"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="ba947-102">ระบุปัญหาเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="ba947-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="ba947-103">การวินิจฉัยเดสก์ท็อปเสมือนของ Windows ใช้ cmdlet ของ PowerShell เพียงรายการเดียว แต่ประกอบด้วยพารามิเตอร์เพิ่มเติมมากมายเพื่อช่วยลดและแยกปัญหา</span><span class="sxs-lookup"><span data-stu-id="ba947-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="ba947-104">เมื่อต้องการเริ่มต้นใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="ba947-104">To get started:</span></span> 

1. <span data-ttu-id="ba947-105">ดาวน์โหลดและนําเข้ามอดูล PowerShell บนเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="ba947-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="ba947-106">For details, see [Windows Virtual Desktop cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="ba947-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="ba947-107">เรียกใช้ cmdlet ต่อไปนี้เพื่อลงชื่อเข้าใช้บัญชีของคุณ:</span><span class="sxs-lookup"><span data-stu-id="ba947-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="ba947-108">ตัวอย่าง: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="ba947-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="ba947-109">**หมายเหตุ:** คิวรีทั้งหมดที่ใช้ PowerShell ต้องมีพารามิเตอร์ -UserName หรือ -ActivityID</span><span class="sxs-lookup"><span data-stu-id="ba947-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="ba947-110">ดูการใช้ Log Analytics เพื่อดูฟีเจอร์การวินิจฉัยเพื่อดู[ความสามารถในการตรวจสอบ](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="ba947-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="ba947-111">เมื่อต้องการกรองกิจกรรมการวินิจฉัยโดยผู้ใช้ ให้เรียกใช้ cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ba947-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="ba947-112">ตัวอย่าง: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="ba947-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="ba947-113">มีรายการตัวกรองที่คุณสามารถเรียกใช้เพื่อวินิจฉัยปัญหา</span><span class="sxs-lookup"><span data-stu-id="ba947-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="ba947-114">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการวินิจฉัยปัญหา ให้ดู ระบุ[และวินิจฉัยปัญหาเดสก์ท็อปเสมือนของ Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="ba947-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="ba947-115">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อผิดพลาดทั่วไป ให้ดูที่ [เซนารีข้อผิดพลาด](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="ba947-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
