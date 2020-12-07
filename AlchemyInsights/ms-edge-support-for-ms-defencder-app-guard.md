---
title: การสนับสนุน microsoft Edge สำหรับ Microsoft Defender Guard แอปพลิเคชัน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584008"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="8641c-102">การสนับสนุน microsoft Edge สำหรับ Microsoft Defender Guard แอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="8641c-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="8641c-103">ได้รับการออกแบบมาสำหรับ Windows 10 และ Microsoft Edge, Guard ของแอปพลิเคชันใช้วิธีการแยกฮาร์ดแวร์ที่ช่วยให้ผู้ใช้นำทางไปยังไซต์ที่ไม่น่าเชื่อถือจากภายในที่แยก, Hyper V –เปิดใช้งานคอนเทนเนอร์ที่แยกออกจากระบบปฏิบัติการโฮสต์</span><span class="sxs-lookup"><span data-stu-id="8641c-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="8641c-104">ผู้ดูแลระบบขององค์กรจะกำหนดรายการของเว็บไซต์ที่เชื่อถือได้ทรัพยากร cloud และเครือข่ายภายใน</span><span class="sxs-lookup"><span data-stu-id="8641c-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="8641c-105">เมื่อผู้ใช้เยี่ยมชมไซต์ที่ไม่ได้อยู่ในรายการ Microsoft Edge จะเปิดไซต์ในคอนเทนเนอร์</span><span class="sxs-lookup"><span data-stu-id="8641c-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="8641c-106">ซึ่งหมายความว่าถ้าไซต์ดังกล่าวออกมาเป็นอันตรายแล้วพีซีโฮสต์จะยังคงได้รับการป้องกันและผู้โจมตีจะไม่สามารถเข้าถึงข้อมูลขององค์กรได้</span><span class="sxs-lookup"><span data-stu-id="8641c-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="8641c-107">การติดตั้งส่วนขยายในคอนเทนเนอร์ได้รับการสนับสนุนจาก Microsoft Edge เวอร์ชัน๘๑และสามารถควบคุมได้ผ่านทางนโยบาย</span><span class="sxs-lookup"><span data-stu-id="8641c-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="8641c-108">ที่อยู่ updateURL ที่ได้รับการใช้ในนโยบาย ExtensionInstallForcelist ควรถูกเพิ่มเป็นทรัพยากรที่เป็นกลางในนโยบายการแยกเครือข่ายที่ใช้โดย Guard ของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="8641c-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="8641c-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่[Microsoft Edge สนับสนุนสำหรับ Microsoft Defender Guard แอปพลิเคชัน](https://go.microsoft.com/fwlink/?linkid=2134229)</span><span class="sxs-lookup"><span data-stu-id="8641c-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
