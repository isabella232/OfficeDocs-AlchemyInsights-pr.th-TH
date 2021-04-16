---
title: การเลิกใช้ Exchange PowerShell และการรับรองความถูกต้องพื้นฐาน
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813491"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="1314d-102">การเลิกใช้ Exchange PowerShell และการรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="1314d-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="1314d-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="1314d-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="1314d-104">โมดูล PowerShell V2 ไม่ได้ใช้การรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="1314d-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="1314d-105">โปรดทราบว่า การรับรองความถูกต้องพื้นฐานยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1314d-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="1314d-106">โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องแบบใหม่เพื่อสร้างการเชื่อมต่อเพื่อเปิดใช้งาน Cmdlet V2 ที่ใช้ REST ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="1314d-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="1314d-107">นอกเหนือจาก cmdlets V2 แล้ว ยังช่วยให้คุณเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) ที่เก่ากว่าซึ่งต้องใช้เซสชัน PowerShell ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="1314d-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="1314d-108">การสร้างเซสชัน RPS บนเครื่อง Windows ต้องใช้ WinRM BasicAuth เพื่อเปิดใช้งานบนเครื่องไคลเอ็นต์แม้ว่าโมดูลจะใช้กลไกการรับรองความถูกต้องแบบใหม่เพื่อรับรองความถูกต้องของบริการ</span><span class="sxs-lookup"><span data-stu-id="1314d-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="1314d-109">ไปป์ไลน์การรับรองความถูกต้องพื้นฐาน WinRM จะใช้ในการส่งโทเค็นการรับรองความถูกต้องแบบใหม่</span><span class="sxs-lookup"><span data-stu-id="1314d-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="1314d-110">ถ้าการรับรองความถูกต้องพื้นฐาน WinRM ถูกปิดใช้งานบนเครื่องไคลเอ็นต์ cmdlets V2 ใหม่จะยังคงสามารถใช้งานต่อไปได้ (แต่ cmdlet RPS ที่เก่ากว่าจะไม่แสดง)</span><span class="sxs-lookup"><span data-stu-id="1314d-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
