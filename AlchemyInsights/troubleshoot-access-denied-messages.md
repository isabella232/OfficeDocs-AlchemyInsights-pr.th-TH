---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704913"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="93b0e-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ</span><span class="sxs-lookup"><span data-stu-id="93b0e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="93b0e-103">ถ้ามีใครบางคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่แชร์ใน SharePoint ผู้ดูแลไซต์คอลเลกชันอาจเปิดใช้งาน "โหมดการจํากัดการเข้าถึงสิทธิ์การเข้าถึงของผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="93b0e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="93b0e-104">เมื่อต้องการปิดใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="93b0e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="93b0e-105">เรียกดูไซต์ คลิกไอคอน การตั้งค่า แล้วคลิก **การตั้งค่า** ไซต์</span><span class="sxs-lookup"><span data-stu-id="93b0e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="93b0e-106">ภายใต้ **การดูแลไซต์คอลเลกชัน** ให้คลิก **ฟีเจอร์ไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="93b0e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="93b0e-107">ถัดจาก **โหมดการจํากัดสิทธิ์การเข้าถึงของผู้ใช้\*\*\*\*ให้คลิกปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="93b0e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="93b0e-108">ข้อความปฏิเสธการเข้าถึงสามารถเกิดขึ้นได้กับโฟลเดอร์ที่แชร์ถ้าไซต์เป็นไซต์การประกาศ</span><span class="sxs-lookup"><span data-stu-id="93b0e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="93b0e-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="93b0e-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="93b0e-110">ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" เมื่อพยายามดูการร้องขอการเข้าถึง ผู้ใช้จะต้องเพิ่มเป็นผู้ดูแลไซต์คอลเลกชันหรือสมาชิกของกลุ่มเจ้าของไซต์</span><span class="sxs-lookup"><span data-stu-id="93b0e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="93b0e-111">For more info, see [Access denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="93b0e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="93b0e-112">ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่ถูกเอาออกจาก Active Directory ภายในองค์กรแล้วถูกเพิ่มกลับ ให้ดูการเข้าถึงถูกปฏิเสธเมื่อบัญชีผู้ใช้ถูกซิงค์กับ[Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="93b0e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

