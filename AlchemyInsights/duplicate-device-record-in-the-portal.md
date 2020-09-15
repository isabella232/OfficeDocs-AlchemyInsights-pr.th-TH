---
title: ระเบียนอุปกรณ์ที่ซ้ำกันในพอร์ทัล
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
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678523"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="4cb81-102">ระเบียนอุปกรณ์ที่ซ้ำกันในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="4cb81-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="4cb81-103">คุณอาจเห็น2ระเบียนสำหรับอุปกรณ์ในพอร์ทัลถ้าอุปกรณ์ไม่ได้รายงานสถานะการจัดการร่วมกับไซต์ตัวจัดการการกำหนดค่าอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="4cb81-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="4cb81-104">เมื่อต้องการตรวจสอบสถานะการจัดการร่วมของอุปกรณ์ให้ตรวจสอบคอลัมน์ที่มีการ **จัดการร่วม** สำหรับอุปกรณ์ในคอนโซลตัวจัดการการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="4cb81-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="4cb81-105">ถ้ามองไม่เห็นคอลัมน์คุณสามารถเพิ่มคอลัมน์ได้โดยการคลิกขวาที่ส่วนหัวของคอลัมน์และเลือกจากรายการ</span><span class="sxs-lookup"><span data-stu-id="4cb81-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="4cb81-106">ค่าที่มีการจัดการร่วมต้องเป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="4cb81-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="4cb81-107">ถ้าค่าไม่ **ใช่**ให้เปิดแอปเพล็ตไคลเอ็นต์การจัดการการตั้งค่าบนอุปกรณ์ไคลเอ็นต์แล้วตรวจสอบคุณสมบัติ **การจัดการร่วม** ในแท็บทั่วไป</span><span class="sxs-lookup"><span data-stu-id="4cb81-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="4cb81-108">ถ้ามีการ **เปิดใช้งาน**ค่านี้จะระบุว่ามีปัญหาเกี่ยวกับการสื่อสารไคลเอ็นต์กับจุดการจัดการ</span><span class="sxs-lookup"><span data-stu-id="4cb81-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="4cb81-109">โปรดตรวจทาน **CcmMessaging** บนอุปกรณ์เพื่อตรวจสอบปัญหาการเชื่อมต่อที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="4cb81-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="4cb81-110">ถ้าค่าถูก **ปิดใช้งาน** และมีการลงทะเบียนอุปกรณ์ใน Intune โปรดตรวจสอบให้แน่ใจว่าอุปกรณ์ได้รับนโยบายการจัดการร่วมด้วยการตรวจสอบ **CoManagementHandler** บนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4cb81-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
