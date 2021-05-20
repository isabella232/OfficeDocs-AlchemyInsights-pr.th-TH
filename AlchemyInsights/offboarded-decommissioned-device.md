---
title: ปัญหาเกี่ยวกับการเอาอุปกรณ์ Offboarded หรืออุปกรณ์ที่ยกเลิกการใช้งานออกจากคลังอุปกรณ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564611"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="7d8aa-102">ปัญหาเกี่ยวกับการเอาอุปกรณ์ Offboarded หรืออุปกรณ์ที่ยกเลิกการใช้งานออกจากคลังอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="7d8aa-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="7d8aa-103">ขณะนี้ Microsoft Defender for Endpoint ไม่อนุญาตให้ลบระเบียนอุปกรณ์ของอุปกรณ์ Offboarded หรือยกเลิกการใช้งานด้วยตนเองออกจากคลังอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="7d8aa-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="7d8aa-104">เพื่อความปลอดภัย อุปกรณ์จะยังคงอยู่ในพอร์ทัลเป็นระเบียนในอดีตเป็นเวลาถึง 180 วัน</span><span class="sxs-lookup"><span data-stu-id="7d8aa-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="7d8aa-105">อย่างไรก็ตาม ข้อมูลอุปกรณ์จะถูกล้างตามช่วงเวลาการเก็บข้อมูลที่คุณกําหนดค่าไว้</span><span class="sxs-lookup"><span data-stu-id="7d8aa-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="7d8aa-106">**หมายเหตุ:** อุปกรณ์ Offboarded หรือยกเลิกการใช้งานจะสลับไปยังสถานะ **ไม่ได้ใช้งาน** โดยอัตโนมัติหลังจากผ่านไปเจ็ดวัน</span><span class="sxs-lookup"><span data-stu-id="7d8aa-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="7d8aa-107">นอกจากนี้ อุปกรณ์ที่ไม่ได้ใช้งานใน 30 วันที่ผ่านมาจะไม่นับเป็นข้อมูลที่สะท้อนถึงคะแนนการเปิดรับการจัดการภัยคุกคามและช่องโหว่หรือคะแนน Microsoft Secure Score for Devices</span><span class="sxs-lookup"><span data-stu-id="7d8aa-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="7d8aa-108">ถ้าคุณยังไม่ต้องการดูอุปกรณ์บางอย่างในมุมมอง คลังอุปกรณ์ ให้ลองวางแท็กอุปกรณ์เพื่อกรองอุปกรณ์ที่ยกเลิกจากมุมมองคลังอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="7d8aa-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="7d8aa-109">สำหรับข้อมูลเพิ่มเติม ให้ดู:</span><span class="sxs-lookup"><span data-stu-id="7d8aa-109">For more information, see:</span></span>

[<span data-ttu-id="7d8aa-110">อุปกรณ์ Offboard จากบริการ Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="7d8aa-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="7d8aa-111">คะแนนแสงในการจัดการภัยคุกคามและช่องโหว่</span><span class="sxs-lookup"><span data-stu-id="7d8aa-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="7d8aa-112">แก้ไขเซนเซอร์ที่ไม่ร้ายแรงใน Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="7d8aa-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="7d8aa-113">วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 1)</span><span class="sxs-lookup"><span data-stu-id="7d8aa-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="7d8aa-114">วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 2)</span><span class="sxs-lookup"><span data-stu-id="7d8aa-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="7d8aa-115">วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 3)</span><span class="sxs-lookup"><span data-stu-id="7d8aa-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




