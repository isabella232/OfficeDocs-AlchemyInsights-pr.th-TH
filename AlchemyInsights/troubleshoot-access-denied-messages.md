---
title: การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050724"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="55a5f-102">การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="55a5f-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="55a5f-103">ถ้ามีคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่ใช้ร่วมกันใน SharePoint ผู้ดูแลชุดเก็บรวบรวมไซต์อาจได้เปิดใช้งาน "จำกัดการเข้าถึงโหมด lockdown สิทธิ์ของผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="55a5f-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="55a5f-104">หากต้องการปิดการทำงานนี้:</span><span class="sxs-lookup"><span data-stu-id="55a5f-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="55a5f-105">เรียกดูไปยังไซต์คลิกไอคอนการตั้งค่าและจากนั้นคลิกการ**ตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="55a5f-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="55a5f-106">ภายใต้การดู**แลไซต์คอลเลกชัน**คลิก**คุณลักษณะของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="55a5f-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="55a5f-107">ถัดจาก**โหมด lockdown สิทธิ์ของผู้ใช้ที่จำกัดการเข้าถึง**คลิ**กปิด**ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="55a5f-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="55a5f-108">ข้อความ Access ถูกปฏิเสธยังสามารถเกิดขึ้นได้สำหรับโฟลเดอร์ที่ใช้ร่วมกันถ้าไซต์เป็นไซต์การประกาศ</span><span class="sxs-lookup"><span data-stu-id="55a5f-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="55a5f-109">สำหรับข้อมูลโปรดดูที่การ[เข้าถึงถูกปฏิเสธเมื่อเข้าถึงโฟลเดอร์ที่ใช้ร่วมกัน](https://go.microsoft.com/fwlink/?linkid=2004317)</span><span class="sxs-lookup"><span data-stu-id="55a5f-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="55a5f-110">ถ้ามีคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" เมื่อพยายามที่จะดูการร้องขอการเข้าถึงผู้ใช้จำเป็นต้องเพิ่มเป็นผู้ดูแลชุดเก็บรวบรวมไซต์หรือสมาชิกของกลุ่มเจ้าของสำหรับไซต์</span><span class="sxs-lookup"><span data-stu-id="55a5f-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="55a5f-111">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[การเข้าถึงถูกปฏิเสธไปยังรายการร้องขอการเข้าถึง](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="55a5f-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="55a5f-112">ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่ถูกเอาออกจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่และจากนั้นเพิ่มกลับมาให้ดู[การเข้าถึงถูกปฏิเสธเมื่อบัญชีผู้ใช้ถูกซิงค์กับ Office ๓๖๕](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="55a5f-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

