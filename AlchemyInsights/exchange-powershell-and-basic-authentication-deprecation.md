---
title: การแลกเปลี่ยน PowerShell และการตรวจสอบพิสูจน์ตัวจริงพื้นฐาน
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
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015708"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="8aa96-102">การแลกเปลี่ยน PowerShell และการตรวจสอบพิสูจน์ตัวจริงพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="8aa96-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="8aa96-103">สําหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่ที่นี่](https://aka.ms/psbasicauth)</span><span class="sxs-lookup"><span data-stu-id="8aa96-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="8aa96-104">โปรดทราบว่าการตรวจสอบความถูกต้องเบื้องต้นยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="8aa96-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="8aa96-105">โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่เพื่อสร้างการเชื่อมต่อสําหรับการเปิดใช้งาน REST-based V2 Cmdlet ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="8aa96-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="8aa96-106">นอกเหนือจาก V2 cmdlets แล้ว ยังช่วยให้คุณเข้าถึง Cmdlets Remote PowerShell (RPS) ที่ต้องใช้เซสชัน PowerShell ระยะไกลเพื่อที่จะสร้าง</span><span class="sxs-lookup"><span data-stu-id="8aa96-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="8aa96-107">สร้างเซสชัน RPS บนเครื่อง Windows ต้องใช้ WinRM BasicAuth เมื่อต้องการเปิดใช้งานบนเครื่องไคลเอนต์แม้ว่าโมดูลใช้กลไกการรับรองความถูกต้องสมัยใหม่เพื่อรับรองความถูกต้องกับบริการ</span><span class="sxs-lookup"><span data-stu-id="8aa96-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="8aa96-108">ขั้นตอนของ WinRM พื้นฐานการรับรองความถูกต้องถูกใช้สําหรับการขนส่งโทเค็นการรับรองความถูกต้องสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="8aa96-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="8aa96-109">ถ้า WinRM Basic รับรองความถูกต้องถูกปิดใช้งานบนเครื่องไคลเอนต์ cmdlet V2 ใหม่จะทํางานต่อไป (แต่ cmdlets RPS เก่าจะไม่)</span><span class="sxs-lookup"><span data-stu-id="8aa96-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
