---
title: ข้อผิดพลาด Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786688"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="5e1ce-102">ข้อผิดพลาด 4c7 ใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5e1ce-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="5e1ce-103">ข้อผิดพลาดนี้เกิดขึ้นเนื่องจาก Microsoft Teams ต้องใช้การรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="5e1ce-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="5e1ce-104">เมื่อคุณปรับใช้ Active Directory Federation Services (AD FS) การรับรองความถูกต้องของฟอร์มจะไม่เปิดใช้งานกับอินทราเน็ตตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="5e1ce-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="5e1ce-105">ถ้าการรับรองความถูกต้องของแบบรวมของ Windows ล้มเหลว คุณจะได้รับพร้อมท์ให้ลงชื่อเข้าใช้โดยใช้การรับรองความถูกต้องของฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="5e1ce-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="5e1ce-106">เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้ Snap-in ของ AD FS Microsoft Management Console (MMC) บนคอมพิวเตอร์ที่มีสําเนาภายในเครื่องของ Active Directory</span><span class="sxs-lookup"><span data-stu-id="5e1ce-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="5e1ce-107">เมื่อต้องการให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="5e1ce-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="5e1ce-108">ในบานหน้าต่างนําทาง ให้เรียกดู **นโยบายการรับรองความถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="5e1ce-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="5e1ce-109">ภายใต้ **การ** แอคชัน ในบานหน้าต่างรายละเอียด ให้เลือก แก้ไข **การรับรองความถูกต้องหลัก** ส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="5e1ce-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="5e1ce-110">บนแท็บ **อินทราเน็ต ให้เลือก\*\*\*\*การรับรองความถูกต้องของฟอร์ม**</span><span class="sxs-lookup"><span data-stu-id="5e1ce-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="5e1ce-111">เลือก **ตกลง** (หรือ **Apply**)</span><span class="sxs-lookup"><span data-stu-id="5e1ce-111">Select **OK** (or **Apply**).</span></span>