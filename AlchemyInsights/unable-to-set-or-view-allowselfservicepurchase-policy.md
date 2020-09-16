---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735218"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="0122b-102">ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="0122b-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="0122b-103">เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณจะได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0122b-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="0122b-104">*HandleError: ล้มเหลวในการเรียกใช้นโยบายผลิตภัณฑ์ด้วย PolicyId ' AllowSelfServicePurchase ' ErrorMessage-การเชื่อมต่อขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*</span><span class="sxs-lookup"><span data-stu-id="0122b-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="0122b-105">การทำเช่นนี้อาจเป็นเพราะเวอร์ชันที่เก่ากว่าของความปลอดภัยของชั้นการขนส่ง (TLS)</span><span class="sxs-lookup"><span data-stu-id="0122b-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="0122b-106">เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณจำเป็นต้องใช้ TLS ๑.๒หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="0122b-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="0122b-107">ให้ลองทำตามขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS ไปยัง๑.๒ตรวจสอบแล้วลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="0122b-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="0122b-108">ที่พร้อมท์คำสั่ง PowerShell (PS C: \) ใส่คำสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS เป็นเวอร์ชัน๑.๒:</span><span class="sxs-lookup"><span data-stu-id="0122b-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="0122b-109">ตรวจสอบว่าโพรโทคอล TLS ถูกใช้งานอยู่ด้วยคำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0122b-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="0122b-110">ลองใช้คำสั่งรับหรืออัปเดตใหม่ตามต้องการ</span><span class="sxs-lookup"><span data-stu-id="0122b-110">Retry the Get or Update commands as needed.</span></span>

