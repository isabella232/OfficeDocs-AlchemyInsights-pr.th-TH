---
title: การโอนย้ายโดเมนระหว่างผู้เช่า
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "7305"
ms.openlocfilehash: d696c9d095fb6b2b374d8c5872e94cc7e32dceb8
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/02/2020
ms.locfileid: "49564988"
---
# <a name="transfer-domain-between-tenants"></a><span data-ttu-id="be1b7-102">การโอนย้ายโดเมนระหว่างผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="be1b7-102">Transfer domain between tenants</span></span>

<span data-ttu-id="be1b7-103">โดเมนแบบกำหนดเองเช่น forthcoffee.com สามารถเอาออกได้ด้วยตนเองจากผู้เช่าหนึ่งรายแล้วตรวจสอบในผู้เช่าใหม่</span><span class="sxs-lookup"><span data-stu-id="be1b7-103">A custom domain such as forthcoffee.com can be manually removed from one tenant and then verified in a new tenant.</span></span>

<span data-ttu-id="be1b7-104">ทำตามขั้นตอนต่อไปนี้เพื่อ[เอาโดเมนออก](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain)</span><span class="sxs-lookup"><span data-stu-id="be1b7-104">Follow these steps to [Remove a domain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain).</span></span> <span data-ttu-id="be1b7-105">จากนั้นในผู้เช่าใหม่ไปที่โดเมน **การตั้งค่า**  >  **Domains**  >  **เพิ่มโดเมน**</span><span class="sxs-lookup"><span data-stu-id="be1b7-105">Then in the new tenant go to **Settings** > **Domains** > **Add domain**.</span></span>

<span data-ttu-id="be1b7-106">สำหรับสถานการณ์ที่ซับซ้อนมากขึ้นให้ดู[ที่การโยกย้ายที่ผู้เช่า-เป็นผู้เช่า Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations)</span><span class="sxs-lookup"><span data-stu-id="be1b7-106">For more complex scenarios, see [Microsoft 365 tenant-to-tenant migrations](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations).</span></span>

<span data-ttu-id="be1b7-107">**นอกจากนี้โปรดทราบ** ว่า:</span><span class="sxs-lookup"><span data-stu-id="be1b7-107">**Also note**:</span></span>
- <span data-ttu-id="be1b7-108">โดเมน onmicrosoft.com เริ่มต้นไม่สามารถลบหรือย้ายไปมาระหว่างผู้เช่าได้</span><span class="sxs-lookup"><span data-stu-id="be1b7-108">The initial onmicrosoft.com domain cannot be deleted or moved between tenants.</span></span>
- <span data-ttu-id="be1b7-109">โดเมนแบบกำหนดเองที่ซื้อจาก Microsoft ไม่สามารถย้ายไปมาระหว่างผู้เช่าได้</span><span class="sxs-lookup"><span data-stu-id="be1b7-109">A custom domain purchased from Microsoft cannot be moved between tenants.</span></span>