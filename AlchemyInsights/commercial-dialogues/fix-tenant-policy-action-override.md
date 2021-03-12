---
title: แก้ไขนโยบายผู้เช่า (การแทนที่การแอคชัน)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748986"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="c43b8-102">แก้ไขนโยบายผู้เช่า (การแทนที่การแอคชัน)</span><span class="sxs-lookup"><span data-stu-id="c43b8-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="c43b8-103">นโยบายการป้องกันสแปมในผู้เช่าของคุณมีผลต่อข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="c43b8-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="c43b8-104">เมื่อต้องการตรวจทานนโยบาย ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c43b8-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="c43b8-105">ไปที่ศูนย์การรักษา [ความปลอดภัยของ office 365 &การปฏิบัติตาม](https://go.microsoft.com/fwlink/p/?linkid=2077143)นโยบาย จากนั้นไปที่ **การป้องกัน**  >    >  [สแปมนโยบายการจัดการ](https://go.microsoft.com/fwlink/?linkid=2101518)ภัยคุกคาม</span><span class="sxs-lookup"><span data-stu-id="c43b8-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="c43b8-106">ตรวจสอบเพื่อดูว่าแหล่งนโยบาย **ระบุถึง** สิ่งต่อไปนี้หรือไม่:  **ข้อความ Add-Xheader/ModifySubject/Redirect/Delete/No action/ ข้อความ BCC**</span><span class="sxs-lookup"><span data-stu-id="c43b8-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="c43b8-107">ถ้าเป็นดังนั้น **บนแท็บ แบบ** ปรับแต่งเอง ให้ตรวจสอบการตั้งค่าของนโยบายที่ได้รับผลกระทบจากข้อความ</span><span class="sxs-lookup"><span data-stu-id="c43b8-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="c43b8-108">อาจเป็นไปได้ว่าการตั้งค่ามาตรฐาน **ที่ปรับใช้** กับลูกค้า Exchange Online Protection ทั้งหมดที่ได้รับผลกระทบจากข้อความ</span><span class="sxs-lookup"><span data-stu-id="c43b8-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="c43b8-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="c43b8-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
