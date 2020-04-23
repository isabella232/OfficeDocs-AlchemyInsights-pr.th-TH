---
title: ทําซ้ําเรกคอร์ดอุปกรณ์ในพอร์ทัล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790176"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="106e2-102">ทําซ้ําเรกคอร์ดอุปกรณ์ในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="106e2-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="106e2-103">คุณอาจเห็น 2 เรกคอร์ดสําหรับอุปกรณ์ในพอร์ทัลถ้าอุปกรณ์ไม่ถูกต้องรายงานสถานะการจัดการร่วมไปยังไซต์ตัวจัดการการตั้งค่าคอนฟิก</span><span class="sxs-lookup"><span data-stu-id="106e2-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="106e2-104">เมื่อต้องการตรวจสอบสถานะการจัดการร่วมของอุปกรณ์ ให้ตรวจทานคอลัมน์**ร่วมที่มีการจัดการ**สําหรับอุปกรณ์ในคอนโซลการจัดการการตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="106e2-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="106e2-105">ถ้ามองไม่เห็นคอลัมน์ คุณอาจเพิ่มคอลัมน์นั้นโดยการคลิกขวาที่ส่วนหัวของคอลัมน์ และเลือกคอลัมน์นั้นจากรายการ</span><span class="sxs-lookup"><span data-stu-id="106e2-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="106e2-106">ค่าที่จัดการร่วมต้องเป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="106e2-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="106e2-107">ถ้าค่าเป็น**ไม่ใช่**เปิดแอปเพล็ตไคลเอ็นต์ตัวจัดการการตั้งค่าคอนฟิกบนอุปกรณ์ไคลเอ็นต์ และตรวจสอบคุณสมบัติ**การจัดการร่วม**ในแท็บทั่วไป</span><span class="sxs-lookup"><span data-stu-id="106e2-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="106e2-108">ถ้าค่าเป็น**Enabled**แสดงว่ามีปัญหากับการสื่อสารกับไคลเอนต์กับจุดการจัดการ</span><span class="sxs-lookup"><span data-stu-id="106e2-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="106e2-109">โปรดตรวจสอบ**CcmMessaging.log**บนอุปกรณ์เพื่อตรวจสอบปัญหาการเชื่อมต่อที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="106e2-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="106e2-110">ถ้า**ค่าถูกปิดใช้งานและอุปกรณ์**ที่ลงทะเบียนใน Intune โปรดตรวจสอบว่า อุปกรณ์ที่ได้รับนโยบายการจัดการร่วม โดยการตรวจสอบ**CoManagementHandler.log**บนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="106e2-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
