---
title: แก้ไขข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690802"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="2ef07-102">แก้ไขข้อความปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="2ef07-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="2ef07-103">ถ้ามีคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่แชร์ใน SharePoint ผู้ดูแลไซต์คอลเลกชันอาจเปิดใช้งาน "การเข้าถึงสิทธิ์ของผู้ใช้ที่ถูกจำกัด"</span><span class="sxs-lookup"><span data-stu-id="2ef07-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="2ef07-104">เมื่อต้องการปิดใช้งานให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="2ef07-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="2ef07-105">เรียกดูไซต์คลิกไอคอนการตั้งค่าแล้วคลิก**การตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="2ef07-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="2ef07-106">ภายใต้การ**ดูแลไซต์คอลเลกชัน**ให้คลิก**ฟีเจอร์ของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="2ef07-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="2ef07-107">ถัดจาก **โหมด lockdown สิทธิ์ของผู้ใช้ในการเข้าถึงที่จำกัด**ให้คลิก **ปิด**ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2ef07-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="2ef07-108">ข้อความที่ถูกปฏิเสธการเข้าถึงยังอาจเกิดขึ้นสำหรับโฟลเดอร์ที่แชร์ถ้าไซต์เป็นไซต์การประกาศ</span><span class="sxs-lookup"><span data-stu-id="2ef07-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="2ef07-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[เข้าถึงถูกปฏิเสธเมื่อเข้าถึงโฟลเดอร์ที่แชร์](https://go.microsoft.com/fwlink/?linkid=2004317)</span><span class="sxs-lookup"><span data-stu-id="2ef07-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="2ef07-110">ถ้ามีใครบางคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" เมื่อพยายามดูการร้องขอการเข้าถึงผู้ใช้จำเป็นต้องเพิ่มเป็นผู้ดูแลไซต์คอลเลกชันหรือสมาชิกของกลุ่มเจ้าของสำหรับไซต์นั้น</span><span class="sxs-lookup"><span data-stu-id="2ef07-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="2ef07-111">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การเข้าถึงถูกปฏิเสธในรายการคำขอการเข้าถึง](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="2ef07-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="2ef07-112">ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่พวกเขาถูกเอาออกจาก Active Directory ภายในองค์กรแล้วเพิ่มกลับมาให้ดู[ที่การเข้าถึงถูกปฏิเสธเมื่อบัญชีผู้ใช้ถูกซิงค์ไปยัง Microsoft ๓๖๕](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="2ef07-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

