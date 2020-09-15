---
title: ลบผู้ใช้ที่ไม่ได้ใช้งานจากเซิร์ฟเวอร์ภายในองค์กร
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680154"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="770af-102">ลบผู้ใช้ที่ไม่ได้ใช้งานจากเซิร์ฟเวอร์ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="770af-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="770af-103">เมื่อต้องการลบผู้ใช้ที่ไม่ได้ใช้งานให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="770af-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="770af-104">บังคับการซิงโครไนซ์ไดเรกทอรีโดยทำตามคำแนะนำใน[ข้อมูลเฉพาะตัวของไฮบริดที่มี Azure Active directory ใช่หรือไม่](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)</span><span class="sxs-lookup"><span data-stu-id="770af-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="770af-105">เมื่อต้องการตรวจสอบการซิงโครไนซ์ไดเรกทอรีให้ดู[ที่ข้อมูลเฉพาะตัวแบบไฮบริดที่มี Azure Active directory คืออะไร](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="770af-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="770af-106">ถ้าการซิงค์ฟังก์ชันอย่างถูกต้องแต่การลบวัตถุไดเรกทอรีที่ใช้งานอยู่ไม่ได้เผยแพร่ไปยัง Azure AD ด้วยตนเองให้เอาวัตถุ orphaned ออกโดยใช้โมดูลของ Active Directory ของ Azure สำหรับ cmdlet ของ Windows PowerShell อย่างใดอย่างหนึ่งดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="770af-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="770af-107">เอาออก-MsolContact</span><span class="sxs-lookup"><span data-stu-id="770af-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="770af-108">เอาออก-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="770af-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="770af-109">เอาออก-MsolUser</span><span class="sxs-lookup"><span data-stu-id="770af-109">Remove-MsolUser</span></span>

    <span data-ttu-id="770af-110">ตัวอย่างเช่นเมื่อต้องการเอา ID ผู้ใช้ที่ไม่ได้ใช้งาน john.smith@contoso.com ออกโดยใช้การซิงโครไนซ์ไดเรกทอรีให้เรียกใช้ cmdlet ดังนี้</span><span class="sxs-lookup"><span data-stu-id="770af-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="770af-111">เอาออก-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="770af-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>