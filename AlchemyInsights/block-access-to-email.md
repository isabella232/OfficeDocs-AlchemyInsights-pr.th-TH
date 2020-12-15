---
title: บล็อกการเข้าถึงอีเมล
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003890"
- "6944"
ms.openlocfilehash: 06079800fee6ce3fb47a1e56c9f4429805d061e2
ms.sourcegitcommit: 72536a4cf4b84235d3a16ffdd428a92f38dd5e87
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680426"
---
# <a name="block-access-to-email"></a><span data-ttu-id="b9012-102">บล็อกการเข้าถึงอีเมล</span><span class="sxs-lookup"><span data-stu-id="b9012-102">Block access to email</span></span>

<span data-ttu-id="b9012-103">เมื่อต้องการบล็อกพนักงานเก่าจากการเข้าถึงบัญชีผู้ใช้อีเมลของพวกเขาใน Microsoft ๓๖๕ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b9012-103">To block former employees from accessing their email accounts in Microsoft 365, follow these steps:</span></span>

1. <span data-ttu-id="b9012-104">ไปที่[ศูนย์การจัดการ Exchange](https://go.microsoft.com/fwlink/?linkid=2138629)</span><span class="sxs-lookup"><span data-stu-id="b9012-104">Go to the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2138629).</span></span>
1. <span data-ttu-id="b9012-105">ภายใต้ **ผู้รับ** ให้คลิก **กล่องจดหมาย**</span><span class="sxs-lookup"><span data-stu-id="b9012-105">Under **Recipients**, click **Mailboxes**.</span></span>
1. <span data-ttu-id="b9012-106">ดับเบิลคลิกที่ชื่อที่ใช้แสดงของผู้ใช้แล้วคลิก **ฟีเจอร์ของกล่องจดหมาย**</span><span class="sxs-lookup"><span data-stu-id="b9012-106">Double-click the user's display name, and then click **mailbox features**.</span></span>
1. <span data-ttu-id="b9012-107">ภายใต้ **อุปกรณ์เคลื่อน** ที่ให้เลือก **ปิดใช้งาน Exchange ActiveSync** และตอบ **ใช่** แล้วเลือก **ปิดใช้งาน OWA สำหรับอุปกรณ์** และตอบ **ใช่**</span><span class="sxs-lookup"><span data-stu-id="b9012-107">Under **Mobile Devices**, select **Disable Exchange ActiveSync** and answer **Yes**, and then select **Disable OWA for Devices** and answer **Yes**.</span></span>
1. <span data-ttu-id="b9012-108">ภายใต้การ **เชื่อมต่ออีเมล** ให้เลือก **ปิดใช้งาน** แล้วตอบ **ใช่**</span><span class="sxs-lookup"><span data-stu-id="b9012-108">Under **Email Connectivity**, select **Disable** and answer **Yes**.</span></span>
1. <span data-ttu-id="b9012-109">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b9012-109">Click **Save**.</span></span>
