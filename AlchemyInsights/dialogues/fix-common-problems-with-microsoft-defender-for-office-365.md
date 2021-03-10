---
title: แก้ไขปัญหาทั่วไปเกี่ยวกับ Microsoft Defender for Office 365
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695630"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="6cd90-102">แก้ไขปัญหาทั่วไปเกี่ยวกับ Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="6cd90-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="6cd90-103">ต่อไปนี้เป็นวิธีแก้ไขปัญหาทั่วไปบางอย่างของ Microsoft Defender for Office 365:</span><span class="sxs-lookup"><span data-stu-id="6cd90-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="6cd90-104">**การหน่วงเวลาข้อความ:** ถ้าคุณพบปัญหาที่การส่งข้อความล่าช้า คุณจะต้องใช้ตัวเลือกการส่งแบบไดนามิกภายในนโยบายสิ่งที่แนบมาที่ปลอดภัยของคุณ</span><span class="sxs-lookup"><span data-stu-id="6cd90-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="6cd90-105">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[การส่งแบบไดนามิกในนโยบายสิ่งที่แนบมาที่ปลอดภัย](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="6cd90-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="6cd90-106">**รายงานผลลัพธ์ที่เป็นบวกหรือลบที่ผิด:** รายงานข้อความไปยังไมโครซอฟท์โดยใช้ลิงก์นี้:[พอร์ทัลการตอบสนองของ Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="6cd90-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="6cd90-107">**เปิดใช้งานการป้องกันลิงก์ที่ปลอดภัย:**</span><span class="sxs-lookup"><span data-stu-id="6cd90-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="6cd90-108">ลงชื่อเข้าใช้ศูนย์การรักษาความปลอดภัยของ[Office 365 &การปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="6cd90-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="6cd90-109">ไปที่ลิงก์Safe  >  **ของ**  >  **นโยบาย Threat** Management</span><span class="sxs-lookup"><span data-stu-id="6cd90-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="6cd90-110">ภายใต้ **นโยบายที่ปรับใช้กับผู้รับที่ระบุ** ให้เปิดนโยบายที่กําหนดค่าไว้</span><span class="sxs-lookup"><span data-stu-id="6cd90-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="6cd90-111">ภายใต้ **การตั้งค่า** ให้เลือก **ใช้ลิงก์ที่ปลอดภัยกับข้อความที่ส่งภายใน** องค์กร</span><span class="sxs-lookup"><span data-stu-id="6cd90-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
