---
title: แก้ไขนโยบายการเชื่อมต่อ
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750598"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="59b8b-102">แก้ไขนโยบายการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="59b8b-102">Fix connection policy</span></span>

<span data-ttu-id="59b8b-103">อีเมลถูกเครื่องหมายว่าปลอดภัยและส่งไปยังกล่องจดหมายเข้าของผู้ใช้เนื่องจากที่อยู่ IP ของผู้ส่งถูกเครื่องหมายว่าปลอดภัยในนโยบายตัวกรองการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="59b8b-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="59b8b-104">เมื่อต้องการตรวจทานนโยบาย ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="59b8b-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="59b8b-105">ไปที่ศูนย์การรักษา [ความปลอดภัยของ office 365 &การปฏิบัติตาม](https://go.microsoft.com/fwlink/p/?linkid=2077143)นโยบาย จากนั้นไปที่ **การป้องกัน**  >    >  [สแปมนโยบายการจัดการ](https://go.microsoft.com/fwlink/?linkid=2101518)ภัยคุกคาม</span><span class="sxs-lookup"><span data-stu-id="59b8b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="59b8b-106">บนแท็บ **แบบ** ปรับแต่งเอง **ให้เลือกนโยบาย** ตัวกรองการเชื่อมต่อ **แล้วเลือก แก้ไข** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="59b8b-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="59b8b-107">รีวิว **รายการอนุญาต IP**</span><span class="sxs-lookup"><span data-stu-id="59b8b-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="59b8b-108">ดูว่า **มีการเปิดใช้งานรายการ** Safe หรือไม่</span><span class="sxs-lookup"><span data-stu-id="59b8b-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="59b8b-109">Microsoft สมัครใช้งานกับแหล่งข้อมูลของบริษัทอื่นของผู้ส่งที่เชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="59b8b-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="59b8b-110">ถ้า **เปิดใช้งาน** รายการที่ปลอดภัย ผู้ส่งที่เชื่อถือได้เหล่านี้จะไม่ถูกระบุว่าเป็นสแปมโดยไม่ได้ตั้งใจ</span><span class="sxs-lookup"><span data-stu-id="59b8b-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="59b8b-111">ฉันแนะให้เลือกตัวเลือกนี้ เนื่องจากตัวเลือกนี้จะลดจํานวนบวกที่ผิด (จดหมายที่ดีที่จัดประเภทเป็นสแปม) ที่คุณได้รับ</span><span class="sxs-lookup"><span data-stu-id="59b8b-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
