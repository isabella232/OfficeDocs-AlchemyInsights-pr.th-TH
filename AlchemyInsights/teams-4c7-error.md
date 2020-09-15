---
title: ข้อผิดพลาดของทีม4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700222"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="1e08c-102">ข้อผิดพลาด4c7 ในทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e08c-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="1e08c-103">ข้อผิดพลาดนี้เกิดขึ้นเนื่องจากทีม Microsoft จำเป็นต้องมีการรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="1e08c-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="1e08c-104">เมื่อคุณปรับใช้บริการสหพันธรัฐไดเรกทอรีที่ใช้งานอยู่ (AD FS) จะไม่มีการเปิดใช้งานการรับรองความถูกต้องของฟอร์มสำหรับอินทราเน็ตตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="1e08c-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="1e08c-105">ถ้าการรับรองความถูกต้องแบบรวมของ Windows ล้มเหลวคุณจะได้รับพร้อมท์ให้ลงชื่อเข้าใช้โดยใช้การรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="1e08c-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="1e08c-106">เมื่อต้องการแก้ไขปัญหานี้ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้สแน็ปอิน AD FS Microsoft Management Console (MMC) บนคอมพิวเตอร์ที่มีสำเนาของ Active Directory ภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="1e08c-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="1e08c-107">เมื่อต้องการทำเช่นนี้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1e08c-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="1e08c-108">ในบานหน้าต่างนำทางให้เรียกดู**นโยบายการรับรองความถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="1e08c-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="1e08c-109">ภายใต้**การดำเนินการ**ในบานหน้าต่างรายละเอียดให้เลือก**แก้ไขการรับรองความถูกต้องหลักส่วนกลาง**</span><span class="sxs-lookup"><span data-stu-id="1e08c-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="1e08c-110">บนแท็บ**อินทราเน็ต**ให้เลือกการ**รับรองความถูกต้องของฟอร์ม**</span><span class="sxs-lookup"><span data-stu-id="1e08c-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="1e08c-111">เลือก **ตกลง** (หรือ **นำไปใช้**)</span><span class="sxs-lookup"><span data-stu-id="1e08c-111">Select **OK** (or **Apply**).</span></span>