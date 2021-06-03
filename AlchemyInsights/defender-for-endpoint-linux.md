---
title: Microsoft Defender for Endpoint บน Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731977"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="b7d8f-102">Microsoft Defender for Endpoint บน Linux</span><span class="sxs-lookup"><span data-stu-id="b7d8f-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="b7d8f-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span><span class="sxs-lookup"><span data-stu-id="b7d8f-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="b7d8f-104">ดูข้อมูลระบบและการติดตั้งที่:</span><span class="sxs-lookup"><span data-stu-id="b7d8f-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="b7d8f-105">เงื่อนไขเบื้องต้น</span><span class="sxs-lookup"><span data-stu-id="b7d8f-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="b7d8f-106">ความต้องการของระบบ</span><span class="sxs-lookup"><span data-stu-id="b7d8f-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="b7d8f-107">คําแนะนําในการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="b7d8f-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="b7d8f-108">การเชื่อมต่อเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="b7d8f-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="b7d8f-109">ดูคําแนะนําที่:</span><span class="sxs-lookup"><span data-stu-id="b7d8f-109">For instructions, see:</span></span>

- [<span data-ttu-id="b7d8f-110">การกําหนดค่าพร็อกซีของอุปกรณ์และการตั้งค่าการเชื่อมต่ออินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="b7d8f-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="b7d8f-111">ปรับใช้การอัปเดตของ Microsoft Defender for Endpoint บน Linux</span><span class="sxs-lookup"><span data-stu-id="b7d8f-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="b7d8f-112">วิธีกําหนดค่า Microsoft Defender for Endpoint บน Linux</span><span class="sxs-lookup"><span data-stu-id="b7d8f-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="b7d8f-113">การสั่งที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="b7d8f-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="b7d8f-114">ฉันต้องการความช่วยเหลือ!</span><span class="sxs-lookup"><span data-stu-id="b7d8f-114">I need help!</span></span>

<span data-ttu-id="b7d8f-115">ถ้าคุณไม่พบข้อมูล/ความช่วยเหลือที่คุณมองหา ให้ปรับปรุงสตริงการค้นหาของคุณ</span><span class="sxs-lookup"><span data-stu-id="b7d8f-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="b7d8f-116">ก่อนที่จะติดต่อฝ่ายสนับสนุนของ Microsoft โปรดตรวจสอบให้แน่ใจว่าได้รวบรวมข้อมูลที่ต้องใช้เพื่อตรวจสอบปัญหาของคุณ และแนบไปกับตั๋ว</span><span class="sxs-lookup"><span data-stu-id="b7d8f-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="b7d8f-117">ดูขั้นตอนรวบรวมข้อมูลการวินิจฉัย[](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="b7d8f-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>