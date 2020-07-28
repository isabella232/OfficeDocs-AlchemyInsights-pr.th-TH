---
title: สินค้าคงคลังอุปกรณ์ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440479"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="4e3b3-102">สินค้าคงคลังอุปกรณ์ Intun</span><span class="sxs-lookup"><span data-stu-id="4e3b3-102">Intune Device Inventory</span></span>

<span data-ttu-id="4e3b3-103">ใบอุปกรณ์ให้ข้อมูลเชิงลึกของผู้ดูแลระบบในอุปกรณ์ภายใต้การจัดการใน Intun</span><span class="sxs-lookup"><span data-stu-id="4e3b3-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="4e3b3-104">ข้อมูลที่แสดงประกอบด้วย: ฮาร์ดแวร์ แอปพลิเคชันที่ค้นพบสถานะการปฏิบัติตามอุปกรณ์ และสถานะการกําหนดค่าอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4e3b3-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="4e3b3-105">ข้อมูลสินค้าคงคลังสําหรับฮาร์ดแวร์และแอปพลิเคชันที่พบจะถูกรวบรวมในรอบเจ็ดวัน</span><span class="sxs-lookup"><span data-stu-id="4e3b3-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="4e3b3-106">แอปพลิเคชันและองค์ประกอบเฉพาะของฮาร์ดแวร์ที่รายงานจะแตกต่างกันขึ้นอยู่กับระบบปฏิบัติการของอุปกรณ์และไม่ว่าอุปกรณ์จะเป็นส่วนบุคคลหรือองค์กรที่เป็นเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="4e3b3-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="4e3b3-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ดูรายละเอียดของอุปกรณ์ใน Intun](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="4e3b3-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="4e3b3-108">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="4e3b3-108">**FAQ**</span></span>

<span data-ttu-id="4e3b3-109">ถาม: ฉันไม่ได้รับรายการรายการแอปพลิเคชันที่มีในอุปกรณ์ Windows ที่ลงทะเบียน Intun</span><span class="sxs-lookup"><span data-stu-id="4e3b3-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="4e3b3-110">ทำไมล่ะ</span><span class="sxs-lookup"><span data-stu-id="4e3b3-110">Why not?</span></span>

<span data-ttu-id="4e3b3-111">A:ในขณะนี้ เฉพาะแอปสมัยใหม่เท่านั้นที่แสดงรายการสําหรับพีซีที่ใช้ Windows 10 ที่ระบุเป็นอุปกรณ์ของบริษัท</span><span class="sxs-lookup"><span data-stu-id="4e3b3-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="4e3b3-112">Intunเนไม่ได้รวบรวมข้อมูลเกี่ยวกับแอป Win32 ที่ติดตั้งบนอุปกรณ์เหล่านี้</span><span class="sxs-lookup"><span data-stu-id="4e3b3-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="4e3b3-113">ถาม: ทําไมหมายเลขโทรศัพท์จึงไม่เก็บจากอุปกรณ์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="4e3b3-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="4e3b3-114">A: โทรศัพท์ที่จัดหมวดหมู่เป็นอุปกรณ์ของบริษัทใน Intuni จะไม่ถูกระบุด้วยหมายเลขโทรศัพท์เต็มเมื่อตัวอย่างเช่น คุณเรียกใช้รายงานสินค้าคงคลังของอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="4e3b3-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="4e3b3-115">หมายเลขโทรศัพท์ของอุปกรณ์นําคุณเองจะถูกสวมหน้ากากบางส่วนด้วยเครื่องหมายดอกจัน (\*\*\*\*) และแสดงเฉพาะตัวเลขสี่หลักสุดท้าย</span><span class="sxs-lookup"><span data-stu-id="4e3b3-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>