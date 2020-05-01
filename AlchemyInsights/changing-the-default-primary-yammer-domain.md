---
title: การเปลี่ยนโดเมนเริ่มต้น Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991330"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="1f862-102">การเปลี่ยนโดเมนเริ่มต้น/หลัก Yammer</span><span class="sxs-lookup"><span data-stu-id="1f862-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="1f862-103">URL ของ Yammer ประกอบด้วยชื่อโดเมนหลักปัจจุบันสําหรับเครือข่าย Yammer ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1f862-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="1f862-104">ชื่อโดเมนนี้อาจไม่ตรงกับชื่อโดเมนหลักที่กําหนดใน Office 365 หรือโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="1f862-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="1f862-105">มีความแตกต่างในลักษณะการทํางานตามจํานวนโดเมนแบบกําหนดเองที่เพิ่มไปยังผู้เช่า และว่า Yammer ในการกําหนดค่าการสนับสนุน (1 ผู้เช่า: 1 เครือข่าย หรือ 1:1)</span><span class="sxs-lookup"><span data-stu-id="1f862-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="1f862-106">เอกสารเกี่ยวกับ[โดเมน Yammer และ Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains)จะพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="1f862-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="1f862-107">สาเหตุทั่วไปที่คุณเห็นโดเมนที่ไม่ถูกต้องคือ ว่า เครือข่าย Yammer หลายที่มีอยู่ และจําเป็นต้องรวมบัญชี</span><span class="sxs-lookup"><span data-stu-id="1f862-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="1f862-108">[การรวมเครือข่ายลงในเครือข่ายเดียว](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)โดยใช้เครื่องมือการโยกย้ายเครือข่ายเป็นขั้นตอนแรกที่สําคัญ</span><span class="sxs-lookup"><span data-stu-id="1f862-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="1f862-109">ทําขั้นตอนนี้ให้เสร็จก่อนจะตั้งค่าโดเมนหลัก</span><span class="sxs-lookup"><span data-stu-id="1f862-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="1f862-110">**ไม่มีโดเมนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="1f862-110">**No custom domains**</span></span>

<span data-ttu-id="1f862-111">สําหรับผู้เช่าใหม่ โดเมนเริ่มต้น (เช่น fabrikam.onmicrosoft.com) จากผู้เช่าจะถูกใช้สําหรับ Yammer</span><span class="sxs-lookup"><span data-stu-id="1f862-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="1f862-112">โดเมนหลักถูกตั้งค่าเป็นyammer.com/fabrikam.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1f862-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="1f862-113">**โดเมนแบบกําหนดเองเดียว**</span><span class="sxs-lookup"><span data-stu-id="1f862-113">**Single custom domain**</span></span>

<span data-ttu-id="1f862-114">Yammer จะเลือกโดเมนแบบกําหนดเอง (เช่น fabrikam.com) จากผู้เช่าเป็นโดเมนหลักใน Yammer โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1f862-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="1f862-115">มันถูกตั้งค่าเป็นyammer.com/fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="1f862-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="1f862-116">การเปลี่ยนแปลงนี้จะทํา โดยบริการซิงค์โดเมน และอาจใช้เวลาถึง 24 ชั่วโมงจึงจะมีผล</span><span class="sxs-lookup"><span data-stu-id="1f862-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="1f862-117">**โดเมนแบบกําหนดเองหลายโดเมน**</span><span class="sxs-lookup"><span data-stu-id="1f862-117">**Multiple custom domains**</span></span>

<span data-ttu-id="1f862-118">Yammer สามารถมีโดเมนหลักที่แตกต่างจากโดเมนผู้เช่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="1f862-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="1f862-119">เนื่องจากมีหลายโดเมนแบบกําหนดเอง Yammer ไม่พยายามที่จะคาดเดาโดเมนที่ถูกต้องจากที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="1f862-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="1f862-120">คุณต้องเปิดกรณีการสนับสนุนเพื่อร้องขอให้เปลี่ยนชื่อโดเมนหลักเป็นโดเมนหลักที่คุณเลือก</span><span class="sxs-lookup"><span data-stu-id="1f862-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="1f862-121">**ข้อมูลการแก้ไขปัญหาเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="1f862-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="1f862-122">ในบางกรณีโดเมนอาจถูกย้ายระหว่างผู้เช่าและบริการซิงค์โดเมนไม่สามารถทํางานเสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="1f862-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="1f862-123">คุณอาจพบปัญหาการลงชื่อเข้าใช้หรือปัญหาอื่นๆ นอกเหนือจากโดเมนหลักที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1f862-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="1f862-124">เมื่อต้องการแก้ไขปัญหานี้ โดเมนอาจจําเป็นต้องถูกย้ายไปยังเครือข่ายที่ถูกต้อง ด้วยความช่วยเหลือจากฝ่ายสนับสนุนของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="1f862-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="1f862-125">สถานการณ์นี้ต้องการความช่วยเหลือโดยตรง และสามารถใช้เวลาในการแก้ไข โดยเฉพาะอย่างยิ่ง ถ้ามีรายการชื่อโดเมนที่ยาวมาก</span><span class="sxs-lookup"><span data-stu-id="1f862-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="1f862-126">เปิดกรณีการสนับสนุนเพื่อขอความช่วยเหลือเกี่ยวกับการแก้ปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="1f862-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="1f862-127">เมื่อทํางานกับตัวแทนฝ่ายสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="1f862-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="1f862-128">พวกเขาอาจถามคําถามการตรวจสอบเพิ่มเติมเกี่ยวกับโดเมนของคุณหากโดเมนเหล่านั้นถูกเพิ่มไปยังผู้เช่าของคุณ แต่ยังไม่ได้ยืนยันโดย DNS</span><span class="sxs-lookup"><span data-stu-id="1f862-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="1f862-129">โปรดตรวจสอบให้แน่ใจว่าโดเมนได้รับการตรวจสอบโดย DNS เพื่อเพิ่มความเร็วของกระบวนการ</span><span class="sxs-lookup"><span data-stu-id="1f862-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
