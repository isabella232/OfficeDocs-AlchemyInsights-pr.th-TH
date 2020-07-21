---
title: ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198369"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="7ef1a-102">ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7ef1a-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="7ef1a-103">ถ้าคุณได้รับข้อผิดพลาด "AADSTS7000112: แอพลิเคชัน '00000005-0000-0ff1-ce000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005", ปัญหาที่มีอยู่กับบริการหลักภายในโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="7ef1a-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="7ef1a-104">ผู้ดูแลระบบอาจปิดใช้งานบริการหลักเพื่อบล็อกการเข้าถึง Yammer</span><span class="sxs-lookup"><span data-stu-id="7ef1a-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="7ef1a-105">การปิดใช้งานบริการหลักไม่แนะนํา และอาจทําให้เกิดปัญหาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7ef1a-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="7ef1a-106">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการที่ได้รับการสนับสนุนเพื่อบล็อกการเข้าถึงของผู้ใช้ไปยัง Yammer ให้ดูที่[ปิดการเข้าถึง Yammer สําหรับผู้ใช้ Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)</span><span class="sxs-lookup"><span data-stu-id="7ef1a-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="7ef1a-107">เมื่อต้องการแก้ไขปัญหานี้ในเว็บไซต์ Azure และคืนค่าการเข้าถึงของผู้ใช้ไปยัง Yammer:</span><span class="sxs-lookup"><span data-stu-id="7ef1a-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="7ef1a-108">เปิดหน้าไดเรกทอรีที่ใช้งานอยู่ของ Azure และเลือก**โปรแกรมประยุกต์องค์กร**ภายใต้**จัดการ**ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="7ef1a-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="7ef1a-109">พิมพ์**Office 365 Yammer**ในกล่องค้นหา และเลือกชื่อโปรแกรมประยุกต์เพื่อเปิดการตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="7ef1a-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="7ef1a-110">เลือก**คุณสมบัติ**ภายใต้**จัดการ**ในบานหน้าต่างการนําทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="7ef1a-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="7ef1a-111">ตั้งค่าของ**เปิดใช้งานสําหรับผู้ใช้เพื่อลงชื่อเข้าใช้หรือไม่**เป็น**ใช่**แล้วเลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="7ef1a-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="7ef1a-112">ลงชื่อเข้าใช้ Yammer อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7ef1a-112">Sign in to Yammer again.</span></span> <span data-ttu-id="7ef1a-113">คุณอาจต้องล้างคุกกี้</span><span class="sxs-lookup"><span data-stu-id="7ef1a-113">You might need to clear cookies.</span></span>

<span data-ttu-id="7ef1a-114">อีกวิธีหนึ่งคือ เรียกใช้คําสั่ง PowerShell เพื่อตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="7ef1a-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="7ef1a-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่["ขออภัย แต่เรากําลังมีปัญหาในการลงชื่อเข้าใช้คุณ"](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="7ef1a-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 