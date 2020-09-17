---
title: การเปลี่ยนโดเมน Yammer เริ่มต้น
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
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793885"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="f7b77-102">การเปลี่ยนโดเมน Yammer เริ่มต้น/หลัก</span><span class="sxs-lookup"><span data-stu-id="f7b77-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="f7b77-103">URL ของ Yammer มีชื่อโดเมนหลักปัจจุบันสำหรับเครือข่าย Yammer ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f7b77-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="f7b77-104">ชื่อโดเมนนี้อาจไม่ตรงกับชุดชื่อโดเมนหลักใน Office ๓๖๕หรือ Azure AD</span><span class="sxs-lookup"><span data-stu-id="f7b77-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="f7b77-105">มีความแตกต่างในลักษณะการทำงานโดยยึดตามจำนวนของโดเมนแบบกำหนดเองที่เพิ่มลงในผู้เช่าและไม่ว่าจะเป็น Yammer ในการกำหนดค่าที่ได้รับการสนับสนุน (1 ผู้เช่า: 1 เครือข่ายหรือ 1:1)</span><span class="sxs-lookup"><span data-stu-id="f7b77-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="f7b77-106">เอกสารประกอบบน [โดเมน Yammer และ Office ๓๖๕](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) จะพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f7b77-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="f7b77-107">สาเหตุทั่วไปที่คุณเห็นโดเมนที่ไม่ถูกต้องคือว่ามีเครือข่าย Yammer หลายเครือข่ายอยู่แล้วและจำเป็นต้องมีการรวม</span><span class="sxs-lookup"><span data-stu-id="f7b77-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="f7b77-108">[การรวมข้อมูลลงในเครือข่ายเดียว](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) โดยใช้เครื่องมือการโยกย้ายเครือข่ายเป็นขั้นตอนแรกที่สำคัญ</span><span class="sxs-lookup"><span data-stu-id="f7b77-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="f7b77-109">ดำเนินการนี้ให้เสร็จสมบูรณ์ก่อนที่จะพยายามตั้งค่าโดเมนหลักของคุณ</span><span class="sxs-lookup"><span data-stu-id="f7b77-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="f7b77-110">**ไม่มีโดเมนแบบกำหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="f7b77-110">**No custom domains**</span></span>

<span data-ttu-id="f7b77-111">สำหรับผู้เช่าใหม่โดเมนเริ่มต้น (เช่น fabrikam.onmicrosoft.com) จากผู้เช่าจะถูกใช้สำหรับ Yammer</span><span class="sxs-lookup"><span data-stu-id="f7b77-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="f7b77-112">โดเมนหลักถูกตั้งค่าเป็น yammer.com/fabrikam.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f7b77-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="f7b77-113">**โดเมนแบบกำหนดเองเดียว**</span><span class="sxs-lookup"><span data-stu-id="f7b77-113">**Single custom domain**</span></span>

<span data-ttu-id="f7b77-114">Yammer จะเลือกโดเมนแบบกำหนดเองโดยอัตโนมัติ (เช่น fabrikam.com) จากผู้เช่าเป็นโดเมนหลักใน Yammer</span><span class="sxs-lookup"><span data-stu-id="f7b77-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="f7b77-115">ตั้งค่าเป็น yammer.com/fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="f7b77-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="f7b77-116">การเปลี่ยนแปลงนี้ทำโดยบริการการซิงค์โดเมนและอาจใช้เวลาถึง24ชั่วโมงเพื่อให้มีผลใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f7b77-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="f7b77-117">**โดเมนแบบกำหนดเองหลายโดเมน**</span><span class="sxs-lookup"><span data-stu-id="f7b77-117">**Multiple custom domains**</span></span>

<span data-ttu-id="f7b77-118">Yammer สามารถมีโดเมนหลักที่แตกต่างจากโดเมนผู้เช่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f7b77-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="f7b77-119">เนื่องจากมีโดเมนแบบกำหนดเองหลายโดเมน Yammer ไม่พยายามคาดเดาโดเมนที่ถูกต้องจากที่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f7b77-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="f7b77-120">คุณจำเป็นต้องเปิดกรณีการสนับสนุนเพื่อร้องขอว่าชื่อโดเมนหลักจะถูกเปลี่ยนเป็นโดเมนหลักของตัวเลือกของคุณ</span><span class="sxs-lookup"><span data-stu-id="f7b77-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="f7b77-121">**ข้อมูลการแก้ไขปัญหาเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="f7b77-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="f7b77-122">ในบางกรณีโดเมนอาจถูกย้ายไปมาระหว่างผู้เช่าและบริการการซิงค์โดเมนไม่สามารถทำงานได้เสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="f7b77-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="f7b77-123">คุณอาจพบปัญหาในการลงชื่อเข้าใช้หรือปัญหาอื่นๆนอกเหนือจากโดเมนหลักที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f7b77-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="f7b77-124">เมื่อต้องการแก้ไขปัญหานี้โดเมนอาจจำเป็นต้องถูกย้ายไปยังเครือข่ายที่ถูกต้องด้วยความช่วยเหลือจากฝ่ายสนับสนุนของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="f7b77-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="f7b77-125">สถานการณ์นี้จำเป็นต้องมีความช่วยเหลือโดยตรงและอาจต้องใช้เวลาสักครู่ในการแก้ไขโดยเฉพาะถ้ามีรายการชื่อโดเมนที่ยาวมาก</span><span class="sxs-lookup"><span data-stu-id="f7b77-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="f7b77-126">เปิดกรณีสนับสนุนเพื่อรับความช่วยเหลือเกี่ยวกับการแก้ไขปัญหาชนิดเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="f7b77-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="f7b77-127">เมื่อทำงานกับตัวแทนฝ่ายสนับสนุนพวกเขาจะตรวจสอบว่าโดเมนได้รับการตรวจสอบในผู้เช่าภายใต้ตัวควบคุมของคุณ</span><span class="sxs-lookup"><span data-stu-id="f7b77-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="f7b77-128">พวกเขาอาจถามคำถามเพิ่มเติมเกี่ยวกับการตรวจสอบโดเมนของคุณถ้าพวกเขาถูกเพิ่มลงในผู้เช่าของคุณแต่ไม่ได้รับการตรวจสอบโดย DNS</span><span class="sxs-lookup"><span data-stu-id="f7b77-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="f7b77-129">โปรดตรวจสอบให้แน่ใจว่าโดเมนได้รับการตรวจสอบโดย DNS เพื่อเพิ่มความเร็วในการดำเนินการ</span><span class="sxs-lookup"><span data-stu-id="f7b77-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
