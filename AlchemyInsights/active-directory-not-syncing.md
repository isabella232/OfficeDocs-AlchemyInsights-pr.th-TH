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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822870"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="44dd0-102">Active Directory ไม่ซิงค์</span><span class="sxs-lookup"><span data-stu-id="44dd0-102">Active Directory not syncing</span></span>

<span data-ttu-id="44dd0-103">ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์ เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบ Office ระบุว่า "ซิงค์ครั้งล่าสุดเมื่อมากกว่า 3 วันที่ผ่านมา" อาจหมายความว่า AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ไม่เพียงพอที่จะซิงโครไนซ์ได้</span><span class="sxs-lookup"><span data-stu-id="44dd0-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="44dd0-104">การติดตั้ง AADConnect อีกครั้งโดยใช้การตั้งค่าแบบด่วนอาจแก้ไขปัญหาได้อย่างรวดเร็ว ดังนี้</span><span class="sxs-lookup"><span data-stu-id="44dd0-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="44dd0-105">[ดาวน์โหลด AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)เวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="44dd0-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="44dd0-106">[ให้ปฏิบัติตามคําแนะนําในการติดตั้ง](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)แบบด่วน</span><span class="sxs-lookup"><span data-stu-id="44dd0-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="44dd0-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="44dd0-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
