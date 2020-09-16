---
title: การใช้ MIP SKD
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
- "9002266"
- "5631"
ms.openlocfilehash: 76d9113bca6416646c76677ab23e12b0589e8a2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770066"
---
# <a name="using-mip-skd"></a><span data-ttu-id="a5909-102">การใช้ MIP SKD</span><span class="sxs-lookup"><span data-stu-id="a5909-102">Using MIP SKD</span></span>

<span data-ttu-id="a5909-103">เมื่อต้องการใช้ SDK MIP มีหลายขั้นตอนที่จำเป็นในการตั้งค่าและกำหนดค่าการสมัครใช้งาน Office ๓๖๕และเวิร์กสเตชันไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5909-103">To use the MIP SDK, there are several steps needed to setup and configure your Office 365 subscription and client workstation.</span></span> <span data-ttu-id="a5909-104">ขั้นตอนเหล่านี้รวมถึง:</span><span class="sxs-lookup"><span data-stu-id="a5909-104">These steps include:</span></span>

- <span data-ttu-id="a5909-105">ลงทะเบียนสำหรับการสมัครใช้งาน Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="a5909-105">Sign up for an Office 365 subscription.</span></span>
- <span data-ttu-id="a5909-106">กำหนดค่าป้ายความลับ</span><span class="sxs-lookup"><span data-stu-id="a5909-106">Configure sensitivity labels.</span></span>
- <span data-ttu-id="a5909-107">กำหนดค่าเวิร์กสเตชันไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5909-107">Configure your client workstation.</span></span>
- <span data-ttu-id="a5909-108">ลงทะเบียนแอปพลิเคชันไคลเอ็นต์ด้วย Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a5909-108">Register a client application with Azure Active Directory.</span></span>
- <span data-ttu-id="a5909-109">ร้องขอข้อตกลงการรวมการป้องกันข้อมูล (IPIA)</span><span class="sxs-lookup"><span data-stu-id="a5909-109">Request an Information Protection Integration Agreement (IPIA).</span></span>
- <span data-ttu-id="a5909-110">ตรวจสอบให้แน่ใจว่าแอปของคุณมีการรันไทม์ที่จำเป็น</span><span class="sxs-lookup"><span data-stu-id="a5909-110">Ensure your app has the required runtime.</span></span>

<span data-ttu-id="a5909-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนของวิทยานิพนธ์ให้ดูที่การ[ตั้งค่าและกำหนดค่า MIP SDK](https://docs.microsoft.com/information-protection/develop/setup-configure-mip)</span><span class="sxs-lookup"><span data-stu-id="a5909-111">For more information on theses steps, see [Setup and Configure MIP SDK](https://docs.microsoft.com/information-protection/develop/setup-configure-mip).</span></span>

<span data-ttu-id="a5909-112">สำหรับแหล่งข้อมูลเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="a5909-112">For additional resources, see:</span></span>

- [<span data-ttu-id="a5909-113">เอกสารประกอบ SDK การป้องกันข้อมูลของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a5909-113">Microsoft Information Protection SDK Documentation</span></span>](https://docs.microsoft.com/information-protection/develop/)
- [<span data-ttu-id="a5909-114">คู่มือสำหรับนักพัฒนาการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="a5909-114">Azure Information Protection Developer's Guide</span></span>](https://docs.microsoft.com/azure/information-protection/develop/developers-guide)
- [<span data-ttu-id="a5909-115">ดาวน์โหลดชุดการพัฒนาซอฟต์แวร์การป้องกันข้อมูลของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a5909-115">Download Microsoft Information Protection Software Development Kit</span></span>](https://www.microsoft.com/download/details.aspx?id=57392)
- [<span data-ttu-id="a5909-116">การตั้งค่าและการกำหนดค่า SDK การป้องกันข้อมูลของ Microsoft (MIP)</span><span class="sxs-lookup"><span data-stu-id="a5909-116">Microsoft Information Protection (MIP) SDK setup and configuration</span></span>](https://docs.microsoft.com/information-protection/develop/setup-configure-mip)
- [<span data-ttu-id="a5909-117">โค้ด Azure ตัวอย่างสำหรับ MIP SDK</span><span class="sxs-lookup"><span data-stu-id="a5909-117">Azure Code Samples for MIP SDK</span></span>](https://azure.microsoft.com/resources/samples/?sort=0&term=mipsdk)
