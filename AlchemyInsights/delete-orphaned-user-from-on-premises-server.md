---
title: ลบผู้ใช้ที่ถูกละเลยจากเซิร์ฟเวอร์ในสถาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198585"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="021a1-102">ลบผู้ใช้ที่ถูกละเลยจากเซิร์ฟเวอร์ในสถาน</span><span class="sxs-lookup"><span data-stu-id="021a1-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="021a1-103">เมื่อต้องการเอาผู้ใช้ที่ไม่ได้ใช้งาน ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="021a1-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="021a1-104">บังคับให้ซิงโครไนส์ไดเรกทอรี โดยทําตามคําแนะนําใน[รหัสประจําตัวไฮบริดสลีกับไดเรกทอรีที่ใช้งานอยู่ของ Azure คืออะไร](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)</span><span class="sxs-lookup"><span data-stu-id="021a1-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="021a1-105">เมื่อต้องการตรวจสอบการซิงโครไนส์ไดเรกทอรี ให้ดูที่[รหัสประจําตัวไฮบริดสลีกับไดเรกทอรีที่ใช้งานอยู่ของ Azure คืออะไร](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="021a1-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="021a1-106">ถ้าฟังก์ชันซิงค์อย่างถูกต้อง แต่การลบวัตถุไดเรกทอรีที่ใช้งานอยู่ไม่เผยแพร่ไปยังโฆษณา Azure ด้วยตนเองเอาวัตถุที่ถูกละเลย โดยใช้ต่อไปนี้ Azure Active Directory โมดูลสําหรับ Windows PowerShell cmdlets:</span><span class="sxs-lookup"><span data-stu-id="021a1-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="021a1-107">ลบ- msolติดต่อ</span><span class="sxs-lookup"><span data-stu-id="021a1-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="021a1-108">ลบ- Msolกรุ๊ป</span><span class="sxs-lookup"><span data-stu-id="021a1-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="021a1-109">ลบ- msolUser</span><span class="sxs-lookup"><span data-stu-id="021a1-109">Remove-MsolUser</span></span>

    <span data-ttu-id="021a1-110">ตัวอย่างเช่น เมื่อต้องการเอา id ผู้ใช้ที่ถูกjohn.smith@contoso.com orphaned ที่สร้างโดยใช้การซิงโครไนส์ของไดเรกทอรี เรียกใช้ cmdlet:</span><span class="sxs-lookup"><span data-stu-id="021a1-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="021a1-111">ลบ - MsolUser - UserPrincipalname John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="021a1-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>