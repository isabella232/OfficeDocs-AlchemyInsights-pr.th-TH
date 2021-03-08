---
title: ตั้งค่า ClientAccessServerEnabled เป็น True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525959"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="a8b6c-102">ตั้งค่า ClientAccessServerEnabled เป็น True</span><span class="sxs-lookup"><span data-stu-id="a8b6c-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="a8b6c-103">ถ้าคุณไม่สามารถเปิดข้อความอีเมลที่เข้ารหัสลับ และดูสิ่งที่แนบมา **แบบ rpmsg** แทน ให้ปฏิบัติตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a8b6c-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="a8b6c-104">เชื่อมต่อกับ Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a8b6c-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="a8b6c-105">เมื่อต้องการเชื่อมต่อกับ Exchange Online PowerShell คุณต้องลงชื่อเข้าใช้โดยใช้ผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบ Exchange</span><span class="sxs-lookup"><span data-stu-id="a8b6c-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="a8b6c-106">a.</span><span class="sxs-lookup"><span data-stu-id="a8b6c-106">a.</span></span> <span data-ttu-id="a8b6c-107">เปิด Windows PowerShell แล้วเรียกใช้สั่งต่อไปนี้: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="a8b6c-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="a8b6c-108">b.</span><span class="sxs-lookup"><span data-stu-id="a8b6c-108">b.</span></span> <span data-ttu-id="a8b6c-109">ในกล่องโต้ตอบการร้องขอ **ข้อมูลรับรองความถูกต้องของ Windows PowerShell** ให้ใส่บัญชีและรหัสผ่านของที่โรงเรียนหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="a8b6c-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="a8b6c-110">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="a8b6c-110">Click **OK**.</span></span> 

2. <span data-ttu-id="a8b6c-111">เรียกใช้การสั่งต่อไปนี้เพื่อสร้างเซสชันใหม่:</span><span class="sxs-lookup"><span data-stu-id="a8b6c-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="a8b6c-112">a.</span><span class="sxs-lookup"><span data-stu-id="a8b6c-112">a.</span></span> <span data-ttu-id="a8b6c-113">เรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a8b6c-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="a8b6c-114">เรียกใช้ `Get-IRMConfiguration` การสั่ง</span><span class="sxs-lookup"><span data-stu-id="a8b6c-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="a8b6c-115">ตรวจสอบ **การตั้งค่า ClientAccessServerEnabled**</span><span class="sxs-lookup"><span data-stu-id="a8b6c-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="a8b6c-116">a.</span><span class="sxs-lookup"><span data-stu-id="a8b6c-116">a.</span></span> <span data-ttu-id="a8b6c-117">ถ้า **การตั้งค่า ClientAccessServerEnabled** ถูกตั้งค่า **เป็น False** ให้เรียกใช้ cmdlet ต่อไปนี้: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="a8b6c-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="a8b6c-118">ปิดเซสชัน PowerShell ของคุณเสมอด้วยสั่งต่อไปนี้: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="a8b6c-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="a8b6c-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="a8b6c-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

