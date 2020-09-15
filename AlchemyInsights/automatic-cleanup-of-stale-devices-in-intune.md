---
title: การล้างข้อมูลอัตโนมัติของอุปกรณ์เก่าใน Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715040"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="7f0eb-102">การล้างข้อมูลอัตโนมัติของอุปกรณ์เก่าใน Intune</span><span class="sxs-lookup"><span data-stu-id="7f0eb-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="7f0eb-103">Intune ช่วยให้ผู้ดูแลระบบสามารถกำหนดค่าช่วงเวลาระหว่าง๙๐และ๒๗๐วันหลังจากที่อุปกรณ์เก่าจะถูกเอาออกจากบริการ</span><span class="sxs-lookup"><span data-stu-id="7f0eb-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="7f0eb-104">การตั้งค่านี้คือความกว้างขององค์กรและเมื่อเปิดใช้งานแล้วจะมีผลทันที</span><span class="sxs-lookup"><span data-stu-id="7f0eb-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="7f0eb-105">อุปกรณ์ใดก็ตามที่ไม่ได้รับการตรวจสอบในเซิร์ฟเวอร์ Intune สำหรับช่วงเวลาที่เกินกว่าการตั้งค่าจะถูกลบออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="7f0eb-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="7f0eb-106">**หมายเหตุ:** วัตถุอุปกรณ์ MDM เท่านั้นที่มีสิทธิ์สำหรับการดำเนินการล้างข้อมูลนี้</span><span class="sxs-lookup"><span data-stu-id="7f0eb-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="7f0eb-107">วัตถุอุปกรณ์ EAS เท่านั้นที่ถูกแยกออก</span><span class="sxs-lookup"><span data-stu-id="7f0eb-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="7f0eb-108">สำหรับข้อมูลเพิ่มเติมเมื่ออุปกรณ์จะมีสิทธิ์ในการลบโดยยึดตามการตั้งค่าการล้างข้อมูลของอุปกรณ์และ "สถานะ":</span><span class="sxs-lookup"><span data-stu-id="7f0eb-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="7f0eb-109">การตั้งค่า: **ลบอุปกรณ์หลังจากวันที่เช็คอินล่าสุด: ใช่ (ค่าบางค่า (N) ในจำนวนวันที่ระบุ)**</span><span class="sxs-lookup"><span data-stu-id="7f0eb-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="7f0eb-110">โดยยึดตามค่า (N) ที่ได้รับการกำหนดค่าในการตั้งค่าบริการ Intune จะลบอุปกรณ์ในวันที่ที่ระบุหลังจากที่ตรวจสอบล่าสุดเสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="7f0eb-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="7f0eb-111">การตั้งค่า:  **ลบอุปกรณ์หลังจากวันที่เช็คอินล่าสุด: ไม่มี**</span><span class="sxs-lookup"><span data-stu-id="7f0eb-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="7f0eb-112">๑๘๐วันหลังจากที่ใบรับรองอุปกรณ์หมดอายุและไม่มีการต่ออายุอุปกรณ์จะถูกลบ</span><span class="sxs-lookup"><span data-stu-id="7f0eb-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="7f0eb-113">**หมายเหตุ:** ในทั้งสองกรณีอุปกรณ์ต้องลงทะเบียนเสร็จเรียบร้อยแล้วใน Intune</span><span class="sxs-lookup"><span data-stu-id="7f0eb-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="7f0eb-114">การลงทะเบียนจะเกิดขึ้นในระหว่างอุปกรณ์แรกที่เช็คอินด้วยบริการ Intune</span><span class="sxs-lookup"><span data-stu-id="7f0eb-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="7f0eb-115">ถ้าอุปกรณ์ทะเบียนเสร็จเรียบร้อยแล้วเพื่อ Intune แต่ไม่ได้เป็น Intune ที่ลงทะเบียนอุปกรณ์จะถูกลบ๒๗๐วันหลังจากการลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="7f0eb-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="7f0eb-116">(๙๐วันที่จะทำเครื่องหมายว่าอุปกรณ์ถูกเพิกถอนแล้วและอีกวันที่๑๘๐เพื่อลบระเบียน)</span><span class="sxs-lookup"><span data-stu-id="7f0eb-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="7f0eb-117">ไม่มีกลไกที่มีอยู่ในคอนโซล Intune ในขณะนี้เพื่อสร้างวันหมดอายุของใบรับรองอุปกรณ์สำหรับอุปกรณ์ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="7f0eb-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>