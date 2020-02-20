---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158580"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="35e21-102">ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="35e21-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="35e21-103">เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณได้รับข้อความแจ้งความผิดพลาดต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="35e21-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="35e21-104">*HandleError: ไม่สามารถเรียกนโยบายผลิตภัณฑ์ด้วย PolicyId ' AllowSelfServicePurchase ' ErrorMessage-การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*</span><span class="sxs-lookup"><span data-stu-id="35e21-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="35e21-105">ซึ่งอาจเกิดจากการขนส่งเลเยอร์ความปลอดภัย (TLS) รุ่นเก่า</span><span class="sxs-lookup"><span data-stu-id="35e21-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="35e21-106">เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณจำเป็นต้องใช้ TLS ๑.๒หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="35e21-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="35e21-107">ลองทำตามขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS เพื่อ๑.๒ตรวจสอบและลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="35e21-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="35e21-108">ที่พร้อมท์คำสั่ง PowerShell (PS C:\)ป้อนคำสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS รุ่น๑.๒:</span><span class="sxs-lookup"><span data-stu-id="35e21-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="35e21-109">ตรวจสอบโพรโทคอล TLS (s) ที่ใช้กับคำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="35e21-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="35e21-110">ลองรับหรือปรับปรุงคำสั่งตามที่จำเป็น</span><span class="sxs-lookup"><span data-stu-id="35e21-110">Retry the Get or Update commands as needed.</span></span>

