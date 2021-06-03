---
title: การจัดส่งไดรฟ์ในบริการMicrosoft 365นําเข้าของคุณ
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
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731950"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="bf50e-102">การจัดส่งไดรฟ์ในบริการMicrosoft 365นําเข้าของคุณ</span><span class="sxs-lookup"><span data-stu-id="bf50e-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="bf50e-103">ใช้การจัดส่งไดรฟ์โดยการคัดลอก PSTs ลงในฮาร์ดไดรฟ์ แล้วส่งฮาร์ดไดรฟ์ไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="bf50e-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="bf50e-104">เมื่อต้องการเริ่มงาน:</span><span class="sxs-lookup"><span data-stu-id="bf50e-104">To start the job:</span></span>

1. <span data-ttu-id="bf50e-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span><span class="sxs-lookup"><span data-stu-id="bf50e-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="bf50e-106">เลือก **เลือกชนิดงาน** นําเข้า **แล้วเลือก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="bf50e-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="bf50e-107">เมื่อต้องการดูขั้นตอนต่างๆ ของตัวเลือกการนําเข้านี้ **ให้เลือก จัดส่งฮาร์ดไดรฟ์ไปยังหนึ่งในที่ตั้งทางกายภาพ** ของเรา</span><span class="sxs-lookup"><span data-stu-id="bf50e-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="bf50e-108">ต่อไปนี้คือสิ่งที่ควรทราบ:</span><span class="sxs-lookup"><span data-stu-id="bf50e-108">Here are some things to remember:</span></span>

- <span data-ttu-id="bf50e-109">คุณต้องได้รับมอบหมายบทบาทนําเข้าส่งออกกล่องจดหมายในExchange Onlineนําเข้าไฟล์ PST Microsoft 365กล่องจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="bf50e-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="bf50e-110">ประสิทธิภาพการคํานวณอาจได้รับผลกระทบจาก PSTs ที่มีขนาดใหญ่กว่า 20 GB</span><span class="sxs-lookup"><span data-stu-id="bf50e-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="bf50e-111">สนับสนุนเฉพาะไดรฟ์โซลิดสสเตต (SSD) ขนาด 2.5 นิ้ว หรือฮาร์ดไดรฟ์ภายในแบบ SATA II/III ขนาด 2.5 นิ้วหรือ 3.5 นิ้วเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="bf50e-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="bf50e-112">ฮาร์ดไดรฟ์ที่มีไฟล์ PST ต้องถูกเข้ารหัสลับBitLocker</span><span class="sxs-lookup"><span data-stu-id="bf50e-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="bf50e-113">ค่าใช้จ่ายในการนําเข้าไฟล์ PST ไปยังMicrosoft 365กล่องจดหมายที่ใช้การจัดส่งไดรฟ์คือ $2 USD ต่อข้อมูล 1 GB</span><span class="sxs-lookup"><span data-stu-id="bf50e-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="bf50e-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="bf50e-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>