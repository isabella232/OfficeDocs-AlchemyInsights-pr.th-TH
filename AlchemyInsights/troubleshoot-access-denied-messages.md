---
title: การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759819"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="cb619-102">การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="cb619-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="cb619-103">ถ้ามีคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่ใช้ร่วมกันใน SharePoint ผู้ดูแลไซต์คอลเลกชันอาจเปิดใช้งาน "โหมดล็อกสิทธิ์ผู้ใช้แบบจํากัด"</span><span class="sxs-lookup"><span data-stu-id="cb619-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="cb619-104">เมื่อต้องการปิดนี้:</span><span class="sxs-lookup"><span data-stu-id="cb619-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="cb619-105">เรียกดูไซต์ แล้วคลิกไอคอน การตั้งค่า แล้วคลิก**การตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="cb619-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="cb619-106">ภายใต้**การดูแลไซต์คอลเลกชัน**ให้คลิก**ฟีเจอร์ของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="cb619-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="cb619-107">ถัดจาก**โหมดล็อกดาวน์สิทธิ์ของผู้ใช้ที่จํากัด**ให้คลิก**ปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="cb619-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="cb619-108">ข้อความการเข้าถึงถูกปฏิเสธยังสามารถเกิดขึ้นสําหรับโฟลเดอร์ที่ใช้ร่วมกันถ้าไซต์เป็นไซต์การประกาศ</span><span class="sxs-lookup"><span data-stu-id="cb619-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="cb619-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเข้าถึงถูกปฏิเสธเมื่อเข้าถึงโฟลเดอร์ที่แชร์](https://go.microsoft.com/fwlink/?linkid=2004317)</span><span class="sxs-lookup"><span data-stu-id="cb619-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="cb619-110">ถ้ามีคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ"</span><span class="sxs-lookup"><span data-stu-id="cb619-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="cb619-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเข้าถึงถูกปฏิเสธไปยังรายการการร้องขอการเข้าถึง](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="cb619-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="cb619-112">ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่พวกเขาถูกเอาออกจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่ และเพิ่มกลับ แล้ว ดู[การเข้าถึงถูกปฏิเสธเมื่อมีซิงค์บัญชีผู้ใช้กับ Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="cb619-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

