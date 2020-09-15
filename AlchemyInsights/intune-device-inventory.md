---
title: สินค้าคงคลังของอุปกรณ์ Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667897"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="0cdd7-102">สินค้าคงคลังของอุปกรณ์ Intune</span><span class="sxs-lookup"><span data-stu-id="0cdd7-102">Intune Device Inventory</span></span>

<span data-ttu-id="0cdd7-103">อุปกรณ์เบลดมีข้อมูลเชิงลึกของผู้ดูแลลงในอุปกรณ์ภายใต้การจัดการใน Intune บนพื้นฐานต่ออุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="0cdd7-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="0cdd7-104">ข้อมูลที่แสดงได้แก่ฮาร์ดแวร์แอปพลิเคชันที่ค้นพบสถานะการปฏิบัติตามนโยบายของอุปกรณ์และสถานะการกำหนดค่าอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="0cdd7-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="0cdd7-105">ข้อมูลสินค้าคงคลังสำหรับฮาร์ดแวร์และแอปพลิเคชันที่ค้นพบจะถูกรวบรวมไว้ในวงจรเจ็ดวัน</span><span class="sxs-lookup"><span data-stu-id="0cdd7-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="0cdd7-106">แอปพลิเคชันและองค์ประกอบเฉพาะของฮาร์ดแวร์ที่รายงานแตกต่างกันโดยขึ้นอยู่กับระบบปฏิบัติการของอุปกรณ์และว่าอุปกรณ์นั้นเป็นแบบส่วนตัวหรือเป็นองค์กรที่เป็นขององค์กร</span><span class="sxs-lookup"><span data-stu-id="0cdd7-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="0cdd7-107">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ดูรายละเอียดของอุปกรณ์ใน Intune](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="0cdd7-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="0cdd7-108">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="0cdd7-108">**FAQ**</span></span>

<span data-ttu-id="0cdd7-109">Q: ฉันไม่ได้รับรายการสินค้าคงคลังทั้งหมดของแอปพลิเคชันที่มีอยู่ในอุปกรณ์ Windows ที่มีการลงทะเบียน Intune</span><span class="sxs-lookup"><span data-stu-id="0cdd7-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="0cdd7-110">ทำไมล่ะ</span><span class="sxs-lookup"><span data-stu-id="0cdd7-110">Why not?</span></span>

<span data-ttu-id="0cdd7-111">A: ในขณะนี้เฉพาะแอปที่ทันสมัยจะแสดงรายการสำหรับพีซีที่ใช้ Windows 10 ที่ระบุว่าเป็นอุปกรณ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="0cdd7-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="0cdd7-112">Intune ไม่รวบรวมข้อมูลเกี่ยวกับแอป Win32 ที่ติดตั้งบนอุปกรณ์เหล่านี้</span><span class="sxs-lookup"><span data-stu-id="0cdd7-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="0cdd7-113">Q: เหตุใดหมายเลขโทรศัพท์จึงไม่ถูกรวบรวมจากอุปกรณ์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="0cdd7-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="0cdd7-114">A: โทรศัพท์ที่มีการจัดประเภทเป็นอุปกรณ์ขององค์กรใน Intune จะไม่ถูกระบุด้วยหมายเลขโทรศัพท์แบบเต็มของพวกเขาเมื่อตัวอย่างเช่นคุณเรียกใช้รายงานสินค้าคงคลังของอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="0cdd7-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="0cdd7-115">การนำหมายเลขโทรศัพท์ของอุปกรณ์ของคุณเป็นเจ้าของอยู่เสมอด้วยเครื่องหมายดอกจัน (\*\*\*) และแสดงเฉพาะตัวเลขสี่หลักสุดท้าย</span><span class="sxs-lookup"><span data-stu-id="0cdd7-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>