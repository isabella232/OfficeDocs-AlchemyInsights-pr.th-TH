---
title: ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796667"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="7cced-102">ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7cced-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="7cced-103">ถ้าคุณได้รับข้อผิดพลาด "AADSTS7000112: แอปพลิเคชัน ' 00000005-0000-0ff1-ce00-000000000000 ' (Yammer) ถูกปิดใช้งาน" ปัญหาที่มีอยู่ในบริการหลักภายใน Azure AD</span><span class="sxs-lookup"><span data-stu-id="7cced-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="7cced-104">ผู้ดูแลระบบอาจปิดใช้งานหลักของบริการเพื่อบล็อกการเข้าถึง Yammer</span><span class="sxs-lookup"><span data-stu-id="7cced-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="7cced-105">การปิดใช้งานหลักของบริการไม่แนะนำและอาจทำให้เกิดปัญหาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7cced-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="7cced-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการที่ได้รับการสนับสนุนเพื่อบล็อกการเข้าถึงของผู้ใช้ไปยัง Yammer ให้ดูที่[ปิดการเข้าถึง yammer สำหรับผู้ใช้ Microsoft ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)</span><span class="sxs-lookup"><span data-stu-id="7cced-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="7cced-107">เมื่อต้องการแก้ไขปัญหานี้ในพอร์ทัล Azure และคืนค่าการเข้าถึงของผู้ใช้ไปยัง Yammer:</span><span class="sxs-lookup"><span data-stu-id="7cced-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="7cced-108">เปิดหน้าไดเรกทอรีที่ใช้งานอยู่ของ Azure แล้วเลือก **แอปพลิเคชันขององค์กร** ภายใต้ **จัดการ** ในบานหน้าต่างนำทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="7cced-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="7cced-109">พิมพ์ **Office ๓๖๕ Yammer** ในกล่องค้นหาแล้วเลือกชื่อแอปพลิเคชันเพื่อเปิดการตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="7cced-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="7cced-110">เลือก **คุณสมบัติ** ภายใต้ **จัดการ** ในบานหน้าต่างนำทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="7cced-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="7cced-111">ตั้งค่าของการ**เปิดใช้งานสำหรับผู้ใช้ในการลงชื่อเข้าใช้ใช่หรือไม่**เมื่อต้องการ**ใช่**แล้วเลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="7cced-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="7cced-112">ลงชื่อเข้าใช้ Yammer อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7cced-112">Sign in to Yammer again.</span></span> <span data-ttu-id="7cced-113">คุณอาจจำเป็นต้องล้างคุกกี้</span><span class="sxs-lookup"><span data-stu-id="7cced-113">You might need to clear cookies.</span></span>

<span data-ttu-id="7cced-114">อีกวิธีหนึ่งคือเรียกใช้คำสั่ง PowerShell เพื่อตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="7cced-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="7cced-115">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ "ขออภัยแต่เรากำลังมีปัญหาในการลงชื่อเข้าใช้คุณ" เมื่อคุณคลิกไทล์ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="7cced-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 