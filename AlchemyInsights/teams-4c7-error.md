---
title: ข้อผิดพลาดของทีม4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796424"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f9672-102">ข้อผิดพลาด4c7 ใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f9672-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f9672-103">ข้อผิดพลาดนี้เกิดขึ้นเนื่องจาก Microsoft Teams ต้องการการรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="f9672-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f9672-104">เมื่อคุณจัดวางบริการสหพันธรัฐไดเรกทอรีที่ใช้งานอยู่ (AD FS), การรับรองความถูกต้องของฟอร์มไม่ได้เปิดใช้งานสำหรับอินทราเน็ตโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f9672-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f9672-105">ถ้าการรับรองความถูกต้องแบบรวมของ Windows ล้มเหลวคุณได้รับพร้อมท์ให้เข้าสู่ระบบโดยใช้การรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="f9672-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f9672-106">เมื่อต้องการแก้ไขปัญหานี้ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้สแน็ปอินคอนโซลการจัดการ Microsoft FS โฆษณา (MMC) บนคอมพิวเตอร์ที่มีสำเนาของไดเรกทอรีที่ใช้งานอยู่ภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="f9672-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f9672-107">โดยทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f9672-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f9672-108">ในบานหน้าต่างนำทางให้เรียกดู**นโยบายการรับรองความถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="f9672-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f9672-109">ภายใต้**การดำเนินการ**ในบานหน้าต่างรายละเอียดให้เลือก**แก้ไขการรับรองความถูกต้องหลักทั่วโลก**</span><span class="sxs-lookup"><span data-stu-id="f9672-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f9672-110">บนแท็บ**อินทราเน็ต**เลือกการ**รับรองความถูกต้องของฟอร์ม**</span><span class="sxs-lookup"><span data-stu-id="f9672-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f9672-111">เลือก**ตกลง**(หรือ**ใช้**)</span><span class="sxs-lookup"><span data-stu-id="f9672-111">Select **OK** (or **Apply**).</span></span>