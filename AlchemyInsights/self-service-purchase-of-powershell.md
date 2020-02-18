---
title: การซื้อแบบบริการตนเองของ PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091777"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="bdd9d-102">การซื้อแบบบริการตนเองของ PowerShell</span><span class="sxs-lookup"><span data-stu-id="bdd9d-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="bdd9d-103">เมื่อต้องการใช้โมดูล PowerShell MSCommerce คุณจำเป็นต้องติดตั้งบนอุปกรณ์ Windows 10 ด้วย TLS ๑.๒ (ที่ต้องการสิทธิ์ของผู้ดูแลระบบภายในเครื่อง)</span><span class="sxs-lookup"><span data-stu-id="bdd9d-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="bdd9d-104">นำเข้าและเชื่อมต่อกับโมดู MSCommerce</span><span class="sxs-lookup"><span data-stu-id="bdd9d-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="bdd9d-105">เมื่อได้รับพร้อมท์ให้เข้าสู่ระบบคุณจะต้องใช้ข้อมูลประจำตัวของบทบาทผู้ดูแลระบบในการเรียกเก็บเงินสากล</span><span class="sxs-lookup"><span data-stu-id="bdd9d-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="bdd9d-106">ถ้าคุณไม่มี TLS ๑.๒คุณอาจได้รับข้อผิดพลาดต่อไปนี้เมื่อพยายามรับหรือปรับปรุงนโยบาย:</span><span class="sxs-lookup"><span data-stu-id="bdd9d-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="bdd9d-107">*ErrorMessage-การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*</span><span class="sxs-lookup"><span data-stu-id="bdd9d-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



