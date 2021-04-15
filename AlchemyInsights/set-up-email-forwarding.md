---
title: ตั้งค่าการส่งต่ออีเมล
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
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787156"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="f2d0a-102">ตรวจสอบการตั้งค่าการส่งต่ออีเมลของกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="f2d0a-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="f2d0a-103">อันดับแรก ต้องเปิดใช้งานการส่งต่ออีเมลในระดับผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="f2d0a-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="f2d0a-104">ถ้าคุณตั้งค่าการส่งต่ออีเมลบนกล่องจดหมาย แต่ไม่ใช้งานได้ (คุณได้รับข้อผิดพลาด **"550 5.7.520 การเข้าถึง** ถูกปฏิเสธ องค์กรของคุณไม่อนุญาตให้ส่งต่อภายนอก" ) โปรดดู ควบคุมการส่งต่ออีเมลภายนอกโดยอัตโนมัติใน [Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f2d0a-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="f2d0a-105">การตรวจสอบการตั้งค่าการส่งต่ออีเมลบนกล่องจดหมายเป็นเรื่องง่ายๆ!</span><span class="sxs-lookup"><span data-stu-id="f2d0a-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="f2d0a-106">เพียงปฏิบัติตามขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="f2d0a-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="f2d0a-107">ถ้านี่เป็นกล่องจดหมายของผู้ใช้ ให้ไปที่ **ผู้ใช้** \> **ที่ใช้งานอยู่** แล้วเลือกผู้ใช้ที่มีกล่องจดหมายที่คุณส่งต่อ</span><span class="sxs-lookup"><span data-stu-id="f2d0a-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="f2d0a-108">บนแท็บ **จดหมาย** ให้เลือก **จัดการการส่งต่อ** อีเมล</span><span class="sxs-lookup"><span data-stu-id="f2d0a-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="f2d0a-109">ถ้านี่เป็นกล่องจดหมายที่แชร์ ให้ไปที่ **กล่องจดหมาย** \> **ที่แชร์ของ** กลุ่ม แล้วเลือกกล่องจดหมายที่แชร์ที่คุณส่งต่อ</span><span class="sxs-lookup"><span data-stu-id="f2d0a-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="f2d0a-110">เลือก **แก้ไข** เพื่อส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="f2d0a-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="f2d0a-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="f2d0a-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="f2d0a-112">เมื่อต้องการส่งคําแนะนําไปยังผู้ใช้ของคุณเพื่อให้พวกเขาสามารถตั้งค่าการส่งต่ออีเมลในกล่องจดหมายของพวกเขา ให้ชี้ไปที่ ส่งต่อ [อีเมลจาก Microsoft 365 ไปยังบัญชีอีเมล](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)อื่น</span><span class="sxs-lookup"><span data-stu-id="f2d0a-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="f2d0a-113">โปรดทราบว่า คุณสามารถส่งต่อไปยังอีเมลแอดเดรสได้เพียงที่อยู่เดียว</span><span class="sxs-lookup"><span data-stu-id="f2d0a-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="f2d0a-114">ถ้าคุณต้องการตั้งค่าการส่งต่อไปยังกลุ่มบุคคล ให้สร้างรายชื่อการแจกจ่าย (ภายใต้ กลุ่ม )เพิ่มผู้ใช้ของคุณ จากนั้นกําหนดค่าการส่งต่อไปยังกลุ่มนั้น</span><span class="sxs-lookup"><span data-stu-id="f2d0a-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="f2d0a-115">คุณมีพนักงานลาออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f2d0a-115">Do you have an employee leaving?</span></span> <span data-ttu-id="f2d0a-116">ดู [เอาพนักงานเก่าออกจาก Microsoft 365 เพื่อดู](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) ขั้นตอนที่แนะนา</span><span class="sxs-lookup"><span data-stu-id="f2d0a-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>