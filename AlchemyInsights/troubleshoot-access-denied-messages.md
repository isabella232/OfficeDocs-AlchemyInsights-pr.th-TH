---
title: การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500442"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="32bf0-102">การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="32bf0-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="32bf0-103">ถ้าใครบางคนได้รับข้อความ "Access Denied" ไปยังโฟลเดอร์ที่ใช้ร่วมกันใน SharePoint ดูแลไซต์คอลเลกชันอาจใช้งาน "จำกัดผู้ใช้สิทธิ์ lockdown โหมดการเข้าถึง"</span><span class="sxs-lookup"><span data-stu-id="32bf0-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="32bf0-104">เมื่อต้องการปิดใช้งานนี้:</span><span class="sxs-lookup"><span data-stu-id="32bf0-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="32bf0-105">เรียกดูไปยังไซต์ คลิกไอคอนการตั้งค่า และจากนั้น คลิก**การตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="32bf0-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="32bf0-106">ภายใต้การ**ดูแลชุดเก็บรวบรวมไซต์**คลิก**คุณลักษณะของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="32bf0-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="32bf0-107">ถัดจาก**โหมด lockdown สิทธิ์ของผู้ใช้ถูกจำกัดการเข้าถึง**คลิก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="32bf0-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="32bf0-108">ข้อความปฏิเสธการเข้าถึงอาจเกิดขึ้นได้นอกจากนี้สำหรับโฟลเดอร์ที่ใช้ร่วมกันถ้าไซต์นี้เป็นไซต์เผยแพร่</span><span class="sxs-lookup"><span data-stu-id="32bf0-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="32bf0-109">สำหรับรายละเอียด ดู[การเข้าถึงถูกปฏิเสธเมื่อเข้าถึงโฟลเดอร์ที่ใช้ร่วมกัน](https://go.microsoft.com/fwlink/?linkid=2004317)</span><span class="sxs-lookup"><span data-stu-id="32bf0-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="32bf0-110">ถ้ามีใครบางคนได้รับข้อความ "Access Denied" เมื่อพยายามที่จะดูการร้องขอการเข้าถึง ผู้ใช้ต้องถูกเพิ่มเป็นผู้ดูแลชุดเก็บรวบรวมไซต์หรือเป็นสมาชิกของกลุ่มเจ้าของสำหรับไซต์</span><span class="sxs-lookup"><span data-stu-id="32bf0-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="32bf0-111">สำหรับข้อมูลเพิ่มเติม ดู[รายการร้องขอการเข้าถึงการเข้าถึงปฏิเสธ](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="32bf0-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="32bf0-112">ถ้าผู้ใช้ได้รับข้อความ "Access Denied" หลังจากที่พวกเขาได้ถูกเอาออกจากไดเรกทอรีที่ใช้งานอยู่ในสถาน และเพิ่มกลับ ดูการ[เข้าถึงถูกปฏิเสธเมื่อบัญชีผู้ใช้มีซิงค์กับ Office 365](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="32bf0-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

