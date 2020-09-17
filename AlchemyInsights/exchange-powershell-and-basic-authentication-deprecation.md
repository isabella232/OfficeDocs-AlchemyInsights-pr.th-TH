---
title: การแผนการรับรองความถูกต้องของ Exchange PowerShell และ basic
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782994"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="31932-102">การแผนการรับรองความถูกต้องของ Exchange PowerShell และ basic</span><span class="sxs-lookup"><span data-stu-id="31932-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="31932-103">สำหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ Exchange Online PowerShell โดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่นี่](https://aka.ms/exops-docs)</span><span class="sxs-lookup"><span data-stu-id="31932-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="31932-104">โมดูลของ PowerShell V2 ไม่ใช้การรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="31932-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="31932-105">โปรดทราบว่าการรับรองความถูกต้องพื้นฐานยังคงจำเป็นต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="31932-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="31932-106">โมดูลของ PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่ในการสร้างการเชื่อมต่อสำหรับการเปิดใช้งาน Cmdlet ของ Cmdlet V2 ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="31932-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="31932-107">นอกเหนือจาก cmdlet ของ V2 แล้วยังช่วยให้คุณสามารถเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) รุ่นเก่าซึ่งจำเป็นต้องมีเซสชัน PowerShell ระยะไกลที่จะถูกสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="31932-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="31932-108">การสร้างเซสชัน RPS บนเครื่อง Windows ต้องการให้ WinRM BasicAuth เปิดใช้งานบนเครื่องไคลเอ็นต์แม้ว่าโมดูลที่ใช้กลไกการรับรองความถูกต้องที่ทันสมัยในการรับรองความถูกต้องของบริการ</span><span class="sxs-lookup"><span data-stu-id="31932-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="31932-109">ขั้นตอนการรับรองความถูกต้องของ WinRM Basic จะใช้สำหรับการขนส่งโทเค็นการรับรองความถูกต้องที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="31932-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="31932-110">ถ้ามีการปิดใช้งานการรับรองความถูกต้องของ WinRM Basic บนเครื่องไคลเอ็นต์ cmdlet V2 ใหม่จะยังคงทำงาน (แต่ cmdlet ของ RPS ที่เก่ากว่าจะไม่)</span><span class="sxs-lookup"><span data-stu-id="31932-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
