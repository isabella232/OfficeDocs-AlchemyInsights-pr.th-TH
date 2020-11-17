---
title: เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085923"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="a4ad0-102">เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="a4ad0-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="a4ad0-103">ณวันที่31ตุลาคม๒๐๑๘ Microsoft ๓๖๕จะดำเนินการเปลี่ยนไปยัง TLS ๑.๒ต่อไป</span><span class="sxs-lookup"><span data-stu-id="a4ad0-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="a4ad0-104">เริ่มต้นวันที่15ตุลาคม๒๐๒๐ O365 จะเริ่มต้นแผนของ TLS ๑.๐และ๑.๑บนบริการ</span><span class="sxs-lookup"><span data-stu-id="a4ad0-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="a4ad0-105">ไวร์ของการเปลี่ยนแปลงนี้จะดำเนินการต่อไปอีกไม่กี่สัปดาห์และเดือนแต่ลูกค้าควรสันนิษฐานว่าไม่มี TLS 1.0/1.1 การโทรจะทำงานเมื่อมีส่วนร่วมกับ O365 เริ่มต้นวันที่15ตุลาคม๒๐๒๐</span><span class="sxs-lookup"><span data-stu-id="a4ad0-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="a4ad0-106">ตามที่สื่อสารก่อนหน้านี้ (MC126199 ใน Dec ๒๐๑๗, MC128929 ใน Feb ๒๐๑๘, MC186827 ในเดือนกรกฎาคม๒๐๑๙และ MC218794 ในเดือนกรกฎาคม๒๐๒๐) เราจะย้ายบริการออนไลน์ทั้งหมดของเราไปยังการขนส่งชั้นความปลอดภัย (TLS) 1.2 + เพื่อให้การเข้ารหัสลับที่ดีที่สุดและเพื่อให้แน่ใจว่าบริการของเรามีความปลอดภัยมากขึ้นตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="a4ad0-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="a4ad0-107">ลูกค้ายังสามารถเลือกที่จะมี TLS 1.0/1.1 บนเซิร์ฟเวอร์และทรัพยากรของพวกเขาแต่ควรจะมีเฉพาะ TLS ๑.๒หรือสูงกว่าจะทำงานเมื่อมีการโต้ตอบกับทรัพยากร O365</span><span class="sxs-lookup"><span data-stu-id="a4ad0-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="a4ad0-108">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงเหล่านี้โปรดดู[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)และ[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a4ad0-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  