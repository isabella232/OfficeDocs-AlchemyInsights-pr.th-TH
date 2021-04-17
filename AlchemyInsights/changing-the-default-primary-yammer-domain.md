---
title: การเปลี่ยนโดเมน Yammer เริ่มต้น
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818019"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="64a24-102">การเปลี่ยนโดเมน Yammer เริ่มต้น/โดเมนหลัก Yammer</span><span class="sxs-lookup"><span data-stu-id="64a24-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="64a24-103">URL ของ Yammer ประกอบด้วยชื่อโดเมนหลักปัจจุบันของเครือข่าย Yammer ของคุณ</span><span class="sxs-lookup"><span data-stu-id="64a24-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="64a24-104">ชื่อโดเมนนี้อาจไม่ตรงกับชื่อโดเมนหลักที่ตั้งใน Office 365 หรือ Azure AD</span><span class="sxs-lookup"><span data-stu-id="64a24-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="64a24-105">มีการความแตกต่างของลักษณะการเกิดขึ้นโดยยึดตามจํานวนโดเมนแบบกําหนดเองที่เพิ่มลงในผู้เช่า และ Yammer อยู่ในการกําหนดค่าที่ได้รับการสนับสนุน (1 ผู้เช่า: 1 เครือข่าย หรือ 1:1)</span><span class="sxs-lookup"><span data-stu-id="64a24-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="64a24-106">เอกสารประกอบเกี่ยวกับ [โดเมน Yammer และ Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="64a24-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="64a24-107">เหตุผลทั่วไปที่คุณเห็นโดเมนที่ไม่ถูกต้องคือมีเครือข่าย Yammer หลายเครือข่ายและต้องถูกรวม</span><span class="sxs-lookup"><span data-stu-id="64a24-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="64a24-108">[การรวมข้อมูลไปยังเครือข่ายเดียวโดยใช้](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) เครื่องมือการโยกย้ายเครือข่ายเป็นขั้นตอนแรกที่สําคัญ</span><span class="sxs-lookup"><span data-stu-id="64a24-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="64a24-109">กรอกข้อมูลนี้ให้เสร็จสมบูรณ์ก่อนที่จะพยายามตั้งค่าโดเมนหลักของคุณ</span><span class="sxs-lookup"><span data-stu-id="64a24-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="64a24-110">**ไม่มีโดเมนแบบปรับแต่งเอง**</span><span class="sxs-lookup"><span data-stu-id="64a24-110">**No custom domains**</span></span>

<span data-ttu-id="64a24-111">For new tenants, the default domain (เช่น. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span><span class="sxs-lookup"><span data-stu-id="64a24-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="64a24-112">โดเมนหลักถูกตั้งค่าเป็น yammer.com/fabrikam.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="64a24-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="64a24-113">**โดเมนแบบปรับแต่งเองเดียว**</span><span class="sxs-lookup"><span data-stu-id="64a24-113">**Single custom domain**</span></span>

<span data-ttu-id="64a24-114">Yammer จะเลือกโดเมนแบบปรับแต่งเอง (เช่น fabrikam.com) จากผู้เช่าเป็นโดเมนหลักใน Yammer โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="64a24-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="64a24-115">ตั้งค่าเป็น yammer.com/fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="64a24-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="64a24-116">การเปลี่ยนแปลงนี้ถูกสร้างขึ้นโดยบริการการซิงค์โดเมน และอาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้มีผล</span><span class="sxs-lookup"><span data-stu-id="64a24-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="64a24-117">**โดเมนแบบปรับแต่งเองหลายรายการ**</span><span class="sxs-lookup"><span data-stu-id="64a24-117">**Multiple custom domains**</span></span>

<span data-ttu-id="64a24-118">Yammer สามารถมีโดเมนหลักที่แตกต่างจากโดเมนผู้เช่าเริ่มต้นได้</span><span class="sxs-lookup"><span data-stu-id="64a24-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="64a24-119">เนื่องจากมีโดเมนแบบปรับแต่งเองหลายโดเมน Yammer จะไม่พยายามคาดเดาโดเมนที่ถูกต้องจากโดเมนที่พร้อมใช้งานเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="64a24-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="64a24-120">คุณต้องเปิดกรณีสนับสนุนเพื่อขอให้เปลี่ยนชื่อโดเมนหลักเป็นโดเมนหลักที่คุณเลือก</span><span class="sxs-lookup"><span data-stu-id="64a24-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="64a24-121">**ข้อมูลการแก้ไขปัญหาเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="64a24-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="64a24-122">ในบางกรณี โดเมนอาจถูกย้ายไปมาระหว่างผู้เช่าและบริการซิงค์โดเมนไม่สามารถเรียกใช้ได้สเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="64a24-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="64a24-123">คุณอาจพบการลงชื่อเข้าใช้หรือปัญหาอื่นๆ นอกเหนือจากโดเมนหลักที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="64a24-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="64a24-124">เมื่อต้องการแก้ไขปัญหานี้ อาจต้องย้ายโดเมนไปยังเครือข่ายที่ถูกต้องด้วยความช่วยเหลือจากฝ่ายสนับสนุนของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="64a24-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="64a24-125">สถานการณ์นี้ต้องการความช่วยเหลือโดยตรงและอาจใช้เวลาในการแก้ไขปัญหาโดยเฉพาะอย่างยิ่งถ้ามีรายการชื่อโดเมนที่ยาวมาก</span><span class="sxs-lookup"><span data-stu-id="64a24-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="64a24-126">เปิดกรณีสนับสนุนเพื่อรับความช่วยเหลือในการแก้ไขปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="64a24-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="64a24-127">เมื่อต้องใช้งานตัวแทนฝ่ายสนับสนุน พวกเขาจะตรวจสอบว่าโดเมนได้รับการตรวจสอบแล้วบนผู้เช่าภายใต้การควบคุมของคุณ</span><span class="sxs-lookup"><span data-stu-id="64a24-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="64a24-128">พวกเขาอาจถามข้อถามการตรวจสอบเพิ่มเติมเกี่ยวกับโดเมนของคุณถ้าโดเมนถูกเพิ่มลงในผู้เช่าของคุณ แต่ไม่ได้รับการยืนยันโดย DNS</span><span class="sxs-lookup"><span data-stu-id="64a24-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="64a24-129">โปรดตรวจสอบให้แน่ใจว่าโดเมนได้รับการตรวจสอบโดย DNS เพื่อให้กระบวนการรวดเร็วขึ้น</span><span class="sxs-lookup"><span data-stu-id="64a24-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
