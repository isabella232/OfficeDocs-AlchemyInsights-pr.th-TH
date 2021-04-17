---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826110"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e58b4-102">ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="e58b4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e58b4-103">เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e58b4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e58b4-104">*HandleError : ไม่สามารถเรียกใช้นโยบายผลิตภัณฑ์ด้วย PolicyId 'AllowSelfServicePurchase', ErrorMessage - การเชื่อมต่อที่เกี่ยวข้องถูกปิด: เกิดข้อผิดพลาดที่ไม่คาดคิดขึ้นในการส่ง*</span><span class="sxs-lookup"><span data-stu-id="e58b4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e58b4-105">ซึ่งอาจเกิดจาก Transport Layer Security (TLS) เวอร์ชันที่เก่ากว่า</span><span class="sxs-lookup"><span data-stu-id="e58b4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e58b4-106">เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณต้องใช้ TLS 1.2 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e58b4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e58b4-107">ลองขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS เป็น 1.2 ตรวจสอบ และลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e58b4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e58b4-108">ที่พร้อมท์สั่ง PowerShell (PS C: \) ใส่ค่าสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS เป็นเวอร์ชัน 1.2:</span><span class="sxs-lookup"><span data-stu-id="e58b4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e58b4-109">ตรวจสอบโพรโทคอล TLS ที่ใช้อยู่ ด้วยสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e58b4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e58b4-110">ลองสั่ง รับ หรือ อัปเดต ใหม่ตามต้องการ</span><span class="sxs-lookup"><span data-stu-id="e58b4-110">Retry the Get or Update commands as needed.</span></span>

