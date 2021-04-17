---
title: ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820953"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="0359a-102">ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="0359a-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="0359a-103">**วิธีที่ 1**</span><span class="sxs-lookup"><span data-stu-id="0359a-103">**Method 1**</span></span>

1. <span data-ttu-id="0359a-104">ลงชื่อเข้าใช้พอร์ทัล Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0359a-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="0359a-105">ไปที่ **ผู้ใช้ > ผู้ใช้ที่ใช้งานอยู่** (หรือ **กลุ่ม > กล่องจดหมายที่แชร์** ถ้าคุณตั้งค่านี้ในกล่องจดหมายที่แชร์)</span><span class="sxs-lookup"><span data-stu-id="0359a-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="0359a-106">เลือกผู้ใช้ที่มีกล่องจดหมาย Microsoft Exchange</span><span class="sxs-lookup"><span data-stu-id="0359a-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="0359a-107">บนเมนูที่ลอยอยู่ทางด้านขวาให้ไปที่ **การตั้งค่าจดหมาย > การตอบกลับอัตโนมัติ** (ถ้าเป็นกล่องจดหมายที่แชร์ เพียงคลิก **การตอบกลับอัตโนมัติ** บนเมนูที่ลอยอยู่)</span><span class="sxs-lookup"><span data-stu-id="0359a-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="0359a-108">**วิธีที่ 2**</span><span class="sxs-lookup"><span data-stu-id="0359a-108">**Method 2**</span></span>

1. <span data-ttu-id="0359a-109">ลงชื่อเข้าใช้พอร์ทัลผู้ดูแลระบบ Microsoft 365 โดยใช้ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="0359a-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="0359a-110">ขยาย **ศูนย์การจัดการ** จากนั้นคลิก **Exchange**</span><span class="sxs-lookup"><span data-stu-id="0359a-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="0359a-111">คลิกรูปภาพที่มุมขวาบน แล้วคลิก **ผู้ใช้อื่น** จากนั้นเลือกกล่องจดหมายของผู้ใช้ที่คุณต้องการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="0359a-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="0359a-112">ทางด้านซ้าย ให้เลือก **ตัวเลือก** แล้วคลิก **จัดระเบียบอีเมล** จากนั้นคลิก **การตอบกลับอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="0359a-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="0359a-113">**วิธีที่ 3**</span><span class="sxs-lookup"><span data-stu-id="0359a-113">**Method 3**</span></span>

<span data-ttu-id="0359a-114">เรียกใช้ cmdlet ต่อไปนี้ใน Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0359a-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="0359a-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="0359a-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="0359a-116">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ cmdlet นี้ โปรดดู [Set-Msolcompanysettings](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)</span><span class="sxs-lookup"><span data-stu-id="0359a-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
