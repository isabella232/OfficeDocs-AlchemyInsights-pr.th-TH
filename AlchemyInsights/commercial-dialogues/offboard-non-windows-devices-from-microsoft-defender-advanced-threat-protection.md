---
title: Offboard ไม่ใช่อุปกรณ์ Windows จาก Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748485"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c0730-102">Offboard ไม่ใช่อุปกรณ์ Windows จาก Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="c0730-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c0730-103">โดยมีวิธีการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c0730-103">Here's how:</span></span>

1. <span data-ttu-id="c0730-104">ติดตามเอกสารของบริษัทอื่นเพื่อยกเลิกการเชื่อมต่อโซลูชันของบริษัทอื่นจาก Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="c0730-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c0730-105">จากผู้เช่า Azure Active Directory ของคุณ ให้เอาสิทธิ์ออกจากโซลูชันของบริษัทอื่น:</span><span class="sxs-lookup"><span data-stu-id="c0730-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c0730-106">ลงชื่อเข้าใช้พอร์ทัล[Azure](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="c0730-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c0730-107">เลือก **บริการทั้งหมด**  >  **แอปพลิเคชัน Azure Active Directory**  >  **Enterprise**</span><span class="sxs-lookup"><span data-stu-id="c0730-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c0730-108">เลือกแอปพลิเคชันที่คุณต้องการ Offboard</span><span class="sxs-lookup"><span data-stu-id="c0730-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c0730-109">เลือกลบ</span><span class="sxs-lookup"><span data-stu-id="c0730-109">Select **Delete**.</span></span>

<span data-ttu-id="c0730-110">หากต้องการเรียนรู้เพิ่มเติม[โปรดดู Offboard ที่ไม่ใช่อุปกรณ์ Windows](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="c0730-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
