---
title: ระเบียนอุปกรณ์ที่คัดลอกในพอร์ทัล
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814535"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f08bc-102">ระเบียนอุปกรณ์ที่คัดลอกในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="f08bc-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f08bc-103">คุณอาจเห็นระเบียน 2 ระเบียนบนอุปกรณ์ในพอร์ทัลถ้าอุปกรณ์รายงานสถานะการจัดการร่วมไปยังไซต์ตัวจัดการการกําหนดค่าไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f08bc-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f08bc-104">เมื่อต้องการตรวจสอบสถานะการจัดการร่วมของอุปกรณ์ ให้ตรวจสอบคอลัมน์ **ที่มี** การจัดการร่วมของอุปกรณ์ในคอนโซลตัวจัดการการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="f08bc-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f08bc-105">ถ้าไม่เห็นคอลัมน์ คุณอาจเพิ่มคอลัมน์โดยคลิกขวาที่ส่วนหัวของคอลัมน์ แล้วเลือกจากรายการ</span><span class="sxs-lookup"><span data-stu-id="f08bc-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f08bc-106">ค่าที่มีการจัดการ **ร่วมต้องเป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="f08bc-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f08bc-107">ถ้าค่าเป็น **ไม่ใช่** ให้เปิดแอปเพล็ตไคลเอ็นต์ตัวจัดการการกําหนดค่าบนอุปกรณ์ไคลเอ็นต์ และตรวจสอบ **คุณสมบัติ** การจัดการร่วม ในแท็บ ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="f08bc-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f08bc-108">ถ้าค่า ถูก **เปิดใช้งาน** จะระบุปัญหาเกี่ยวกับการสื่อสารไคลเอ็นต์ด้วยจุดการจัดการ</span><span class="sxs-lookup"><span data-stu-id="f08bc-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f08bc-109">โปรดตรวจทาน **CcmMessaging.log** บนอุปกรณ์เพื่อตรวจสอบปัญหาการเชื่อมต่อที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="f08bc-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f08bc-110">ถ้า **ค่าถูกปิดใช้งานและอุปกรณ์** ได้รับการลงทะเบียนใน Intuny โปรดตรวจสอบให้แน่ใจว่าอุปกรณ์ได้รับนโยบายการจัดการร่วมโดยการตรวจสอบ **CoManagementHandler.log** บนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="f08bc-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
