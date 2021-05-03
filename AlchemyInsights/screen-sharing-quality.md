---
title: คุณภาพการแชร์หน้าจอ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125448"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="87112-102">คุณภาพการแชร์หน้าจอ</span><span class="sxs-lookup"><span data-stu-id="87112-102">Screen sharing quality</span></span>

<span data-ttu-id="87112-103">ในกรณีส่วนใหญ่ ปัญหาคุณภาพการแชร์หน้าจอจะลดเป็นแบนด์วิดท์ที่จํากัดจากฝั่งไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="87112-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="87112-104">ไม่มีข้อจํากัดด้านแบนด์วิดท์ Teams จะปรับคุณภาพสื่อให้เหมาะสม รวมถึงความละเอียดวิดีโอสูงสุด 1080p สูงสุด 30fps ของวิดีโอและ 15fps เพื่อเนื้อหา และเสียงความเที่ยงตรงสูง</span><span class="sxs-lookup"><span data-stu-id="87112-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="87112-105">Teamsใช้แบนด์วิดท์ที่ดั้งเดิมอยู่เสมอ และสามารถให้คุณภาพวิดีโอระดับ HD ภายใต้ 1.2Mbps ได้</span><span class="sxs-lookup"><span data-stu-id="87112-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="87112-106">การใช้งานแบนด์วิดท์ตามจริงในการโทรด้วยเสียง/วิดีโอหรือการประชุมแต่ละครั้งจะแตกต่างกันไปตามปัจจัยต่างๆ เช่น เค้าโครงวิดีโอ ความละเอียดของวิดีโอ และเฟรมวิดีโอต่อวินาที</span><span class="sxs-lookup"><span data-stu-id="87112-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="87112-107">เมื่อมีแบนด์วิดท์เพิ่มขึ้น คุณภาพและการใช้งานจะเพิ่มขึ้นเพื่อให้ได้รับประสบการณ์การใช้งานที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="87112-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="87112-108">ตารางนี้อธิบายวิธีการใช้Teamsวิดท์:</span><span class="sxs-lookup"><span data-stu-id="87112-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="87112-109">**สถานการณ์ Bandwidth(ขึ้น/ลง)**</span><span class="sxs-lookup"><span data-stu-id="87112-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="87112-110">การโทรด้วยเสียงแบบเพียร์ทูเพียร์ 30kbs</span><span class="sxs-lookup"><span data-stu-id="87112-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="87112-111">การโทรด้วยเสียงแบบเพียร์ทูเพียร์ 130 นิ้วและการแชร์หน้าจอ</span><span class="sxs-lookup"><span data-stu-id="87112-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="87112-112">การสนทนาทางวิดีโอคุณภาพแบบเพียร์ทูเพียร์ 500kb ที่ 360p ที่ 30fps</span><span class="sxs-lookup"><span data-stu-id="87112-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="87112-113">การสนทนาทางวิดีโอคุณภาพ HD แบบเพียร์ทูเพียร์แบบ 1.2 Mbps ที่มีความละเอียด HD 720p ที่ 30fps</span><span class="sxs-lookup"><span data-stu-id="87112-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="87112-114">การสนทนาทางวิดีโอคุณภาพ HD แบบเพียร์ทูเพียร์แบบ 1.5 Mbps ที่มีความละเอียด HD 1080p ที่ 30fps</span><span class="sxs-lookup"><span data-stu-id="87112-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="87112-115">การสนทนาทางวิดีโอกลุ่ม 500kbps/1Mbps</span><span class="sxs-lookup"><span data-stu-id="87112-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="87112-116">การสนทนาทางวิดีโอแบบ 1Mbps/2Mbps HD Group (วิดีโอ 540p บนหน้าจอ 1080p)</span><span class="sxs-lookup"><span data-stu-id="87112-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="87112-117">ดูข้อมูลเพิ่มเติมที่[เตรียมเครือข่ายองค์กรของคุณMicrosoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="87112-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>