---
title: ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM for a specific domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749733"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="36f6c-102">ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM for a specific domain</span><span class="sxs-lookup"><span data-stu-id="36f6c-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="36f6c-103">ถ้าคุณไม่สามารถสร้างระเบียน DNS ของ DKIM ในศูนย์การจัดการ ให้ลองใช้ Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="36f6c-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="36f6c-104">เมื่อต้องการสร้างระเบียน DNS DKIM โดยใช้ Exchange Online PowerShell ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="36f6c-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="36f6c-105">เปิด Windows PowerShell ในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในลดับที่อธิบายไว้:</span><span class="sxs-lookup"><span data-stu-id="36f6c-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="36f6c-106">a.</span><span class="sxs-lookup"><span data-stu-id="36f6c-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="36f6c-107">b.</span><span class="sxs-lookup"><span data-stu-id="36f6c-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="36f6c-108">c.</span><span class="sxs-lookup"><span data-stu-id="36f6c-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="36f6c-109">ถ้าคุณมีปัญหาในการเชื่อมต่อกับ Exchange Online PowerShell ให้ดู[เชื่อมต่อกับ Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="36f6c-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="36f6c-110">เมื่อคุณเชื่อมต่อกับ Exchange Online PowerShell ให้เรียกใช้การสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="36f6c-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="36f6c-111">เมื่อเรียกใช้การสั่งข้างต้นเสร็จสมบูรณ์แล้ว ให้เรียกใช้สั่งต่อไปนี้เพื่อสิ้นสุดเซสชัน Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="36f6c-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



