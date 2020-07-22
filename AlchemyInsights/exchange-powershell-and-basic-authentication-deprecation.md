---
title: การแลกเปลี่ยน PowerShell และการเลิกใช้การรับรองความถูกต้องพื้นฐาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205214"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="c5af2-102">การแลกเปลี่ยน PowerShell และการเลิกใช้การรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="c5af2-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="c5af2-103">สําหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่ที่นี่](https://aka.ms/exops-docs)</span><span class="sxs-lookup"><span data-stu-id="c5af2-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="c5af2-104">โมดูล PowerShell V2 ไม่ได้ใช้การรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="c5af2-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="c5af2-105">โปรดทราบว่าการรับรองความถูกต้องพื้นฐานยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5af2-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="c5af2-106">โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่เพื่อสร้างการเชื่อมต่อสําหรับการเปิดใช้งาน Cmdlet ของ V2 ที่ใช้ REST ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="c5af2-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="c5af2-107">นอกจาก cmdlet ของ V2 ก็ยังช่วยให้คุณสามารถเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) เก่าซึ่งต้องใช้เซสชัน PowerShell ระยะไกลที่จะจัดตั้งขึ้น</span><span class="sxs-lookup"><span data-stu-id="c5af2-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="c5af2-108">การสร้างเซสชัน RPS บนเครื่อง Windows ต้อง WinRM BasicAuth เพื่อเปิดใช้งานบนเครื่องไคลเอนต์แม้ว่าโมดูลใช้กลไกการรับรองความถูกต้องแบบสมัยใหม่เพื่อรับรองความถูกต้องกับบริการ</span><span class="sxs-lookup"><span data-stu-id="c5af2-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="c5af2-109">ขั้นตอนการตรวจสอบพื้นฐาน WinRM ถูกใช้สําหรับการขนส่งโทเค็นการรับรองความถูกต้องสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="c5af2-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="c5af2-110">ถ้า WinRM พื้นฐานการรับรองความถูกต้องถูกปิดใช้งานบนเครื่องไคลเอ็นต์ cmdlets V2 ใหม่จะยังคงทํางานต่อไป (แต่ cmdlet ของ RPS เก่าจะไม่)</span><span class="sxs-lookup"><span data-stu-id="c5af2-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
