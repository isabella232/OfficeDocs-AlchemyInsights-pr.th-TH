---
title: การกําหนดค่าข้อยกเว้นMicrosoft Defender ATPสแกน
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543704"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="87b24-102">การกําหนดค่าข้อยกเว้นMicrosoft Defender ATPสแกน</span><span class="sxs-lookup"><span data-stu-id="87b24-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="87b24-103">โดยทั่วไปแล้ว คุณสามารถยกเว้นส่วนขยายของไฟล์และโฟลเดอร์บางรายการจากMicrosoft Defender ATPสแกนได้</span><span class="sxs-lookup"><span data-stu-id="87b24-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="87b24-104">คุณยังสามารถกําหนดค่าการยกเว้นไฟล์ที่เปิดโดยกระบวนการบางอย่างได้</span><span class="sxs-lookup"><span data-stu-id="87b24-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="87b24-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and Configure [exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="87b24-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="87b24-106">เมื่อต้องการกําหนดค่าการยกเว้น **Windows Server 2016 และ 2019** ให้ดูที่ กําหนดค่าโปรแกรมป้องกันไวรัสของ Microsoft Defender [แยกออกWindowsบนเซิร์ฟเวอร์](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="87b24-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="87b24-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="87b24-107">**Mac**</span></span>

<span data-ttu-id="87b24-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="87b24-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="87b24-109">**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้</span><span class="sxs-lookup"><span data-stu-id="87b24-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="87b24-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="87b24-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="87b24-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="87b24-111">**Linux**</span></span>

<span data-ttu-id="87b24-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="87b24-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="87b24-113">**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้</span><span class="sxs-lookup"><span data-stu-id="87b24-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="87b24-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="87b24-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 