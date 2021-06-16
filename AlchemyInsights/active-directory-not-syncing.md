---
title: Active Directory ไม่ซิงค์
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930994"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="36a38-102">Active Directory ไม่ซิงค์</span><span class="sxs-lookup"><span data-stu-id="36a38-102">Active Directory not syncing</span></span>

<span data-ttu-id="36a38-103">ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์ เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบของ Office ระบุว่า "ซิงค์ครั้งล่าสุดนานกว่า 3 วันที่ผ่านมา" อาจเป็นเพราะ AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ที่ไม่เพียงพอที่จะซิงโครไนซ์ได้</span><span class="sxs-lookup"><span data-stu-id="36a38-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="36a38-104">การติดตั้ง AADConnect อีกครั้งโดยใช้การตั้งค่าแบบด่วนอาจช่วยแก้ไขปัญหาได้อย่างรวดเร็ว ดังนี้</span><span class="sxs-lookup"><span data-stu-id="36a38-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="36a38-105">[ดาวน์โหลด AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)เวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="36a38-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="36a38-106">[ให้ปฏิบัติตามคําแนะนําในการติดตั้ง](/azure/active-directory/hybrid/how-to-connect-install-express)แบบด่วน</span><span class="sxs-lookup"><span data-stu-id="36a38-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="36a38-107">ต้องเชื่อมต่อ Azure AD Windows Server 2012 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="36a38-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="36a38-108">เซิร์ฟเวอร์นี้ต้องถูกรวมโดเมนและอาจเป็นตัวควบคุมโดเมนหรือเซิร์ฟเวอร์สมาชิก</span><span class="sxs-lookup"><span data-stu-id="36a38-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="36a38-109">For a full list of Azure AD เชื่อมต่อ requirements and pre-requisites, review [Prerequisites for Azure AD เชื่อมต่อ](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="36a38-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="36a38-110">For more information about AADConnect service accounts, see [Azure AD เชื่อมต่อ: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="36a38-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
