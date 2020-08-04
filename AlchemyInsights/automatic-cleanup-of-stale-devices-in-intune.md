---
title: การล้างข้อมูลอัตโนมัติของอุปกรณ์เก่าใน Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555736"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="a98e2-102">การล้างข้อมูลอัตโนมัติของอุปกรณ์เก่าใน Intun</span><span class="sxs-lookup"><span data-stu-id="a98e2-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="a98e2-103">Intuna ช่วยให้ผู้ดูแลระบบสามารถกําหนดค่าช่วงเวลาระหว่าง 90 และ 270 วันหลังจากที่อุปกรณ์เก่าที่จะถูกลบออกจากบริการ</span><span class="sxs-lookup"><span data-stu-id="a98e2-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="a98e2-104">การตั้งค่านี้เป็นองค์กรกว้างและเมื่อเปิดใช้งานจะมีผลทันที</span><span class="sxs-lookup"><span data-stu-id="a98e2-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="a98e2-105">อุปกรณ์ใดๆ ที่ไม่ได้เช็คอินในเซิร์ฟเวอร์ Intuner สําหรับรอบระยะเวลาที่เกินการตั้งค่าจะถูกลบอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="a98e2-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="a98e2-106">**หมายเหตุ** เฉพาะวัตถุอุปกรณ์ MDM เท่านั้นที่มีสิทธิ์สําหรับการดําเนินการล้างข้อมูลนี้</span><span class="sxs-lookup"><span data-stu-id="a98e2-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="a98e2-107">EAS เท่านั้นอุปกรณ์วัตถุจะถูกแยกออก</span><span class="sxs-lookup"><span data-stu-id="a98e2-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="a98e2-108">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกรณีที่อุปกรณ์มีสิทธิ์ในการลบตามการตั้งค่าการล้างข้อมูลอุปกรณ์และ "สถานะ":</span><span class="sxs-lookup"><span data-stu-id="a98e2-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="a98e2-109">การตั้งค่า:**ลบอุปกรณ์หลังจากวันที่เช็คอินครั้งล่าสุด: ใช่ (ค่าบางค่า (N) เป็นวันๆ)**</span><span class="sxs-lookup"><span data-stu-id="a98e2-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="a98e2-110">ขึ้นอยู่กับค่า (N) ที่กําหนดค่าในการตั้งค่า บริการ Intunn ลบอุปกรณ์ในวันที่ระบุหลังจากที่เช็คอินเสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="a98e2-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="a98e2-111">การตั้งค่า:**ลบอุปกรณ์หลังจากวันเช็คอินล่าสุด: ไม่**</span><span class="sxs-lookup"><span data-stu-id="a98e2-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="a98e2-112">180 วันหลังจากใบรับรองอุปกรณ์หมดอายุและไม่ได้ต่ออายุอุปกรณ์จะถูกลบออก</span><span class="sxs-lookup"><span data-stu-id="a98e2-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="a98e2-113">**หมายเหตุ** ในทั้งสองกรณี อุปกรณ์ต้องลงทะเบียนเรียบร้อยแล้วใน Intun</span><span class="sxs-lookup"><span data-stu-id="a98e2-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="a98e2-114">การลงทะเบียนเกิดขึ้นระหว่างการตรวจสอบอุปกรณ์แรกกับบริการ Intun</span><span class="sxs-lookup"><span data-stu-id="a98e2-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="a98e2-115">หากอุปกรณ์ลงทะเบียนสําเร็จเพื่อ Intun</span><span class="sxs-lookup"><span data-stu-id="a98e2-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="a98e2-116">(90 วันในการทําเครื่องหมายอุปกรณ์ว่ายกเลิกแล้ว จากนั้นอีก 180 วันเพื่อลบระเบียน)</span><span class="sxs-lookup"><span data-stu-id="a98e2-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="a98e2-117">ไม่มีกลไกอยู่ในคอนโซล Intuni เพื่อสร้างวันหมดอายุของการรับรองอุปกรณ์สําหรับอุปกรณ์ใด ๆ</span><span class="sxs-lookup"><span data-stu-id="a98e2-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>