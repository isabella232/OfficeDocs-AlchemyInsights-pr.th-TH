---
title: การซื้อ PowerShell แบบบริการตนเอง
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797740"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="0af3f-102">การซื้อ PowerShell แบบบริการตนเอง</span><span class="sxs-lookup"><span data-stu-id="0af3f-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="0af3f-103">เมื่อต้องการใช้มอดูล MSCommerce PowerShell คุณต้องติดตั้งโมดูลนั้นบนอุปกรณ์ Windows 10 ที่มี TLS 1.2 (ต้องมีสิทธิ์ระดับผู้ดูแลระบบภายใน)</span><span class="sxs-lookup"><span data-stu-id="0af3f-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="0af3f-104">นําเข้าและเชื่อมต่อกับมอดูล MSCommerce</span><span class="sxs-lookup"><span data-stu-id="0af3f-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="0af3f-105">เมื่อได้รับพร้อมท์ให้เข้าสู่ระบบ คุณจะต้องใช้ข้อมูลรับรองบทบาทผู้ดูแลระบบส่วนกลางหรือการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="0af3f-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="0af3f-106">ถ้าคุณไม่มี TLS 1.2 คุณอาจได้รับข้อผิดพลาดต่อไปนี้เมื่อพยายามรับหรืออัปเดตนโยบาย</span><span class="sxs-lookup"><span data-stu-id="0af3f-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="0af3f-107">*ErrorMessage -การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด: เกิดข้อผิดพลาดที่ไม่คาดคิดขึ้นใน* การส่ง</span><span class="sxs-lookup"><span data-stu-id="0af3f-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



