---
title: ตรวจสอบการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538795"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="036dc-102">ตรวจสอบการเข้าถึงแบบมีเงื่อนไขสำหรับการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="036dc-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="036dc-103">ผู้ใช้ที่เป็นเป้าหมาย มีการเข้าถึงแบบมีเงื่อนไขจะได้รับอีเมลการแจ้งเตือนถ้าพวกเขาไม่ตรงกับความต้องการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="036dc-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="036dc-104">เมื่อต้องการแก้ไข เราขอแนะนำการแก้ไขปัญหาต่อไปนี้อย่างใดอย่างหนึ่ง:</span><span class="sxs-lookup"><span data-stu-id="036dc-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="036dc-105">ถ้าอุปกรณ์เป็น presumed เมื่อต้องการลงทะเบียน คำแนะนำผู้ใช้ไปยังแอพลิเคชันเว็บไซต์บริษัท และตรวจสอบว่า จะปรากฏอยู่ในเว็บไซต์บริษัท</span><span class="sxs-lookup"><span data-stu-id="036dc-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="036dc-106">หากโปรแกรมไม่ ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="036dc-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="036dc-107">ในเว็บไซต์ Azure ไป**Intune\>ปฏิบัติตามกฎระเบียบอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="036dc-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="036dc-108">ภายใต้**จอภาพ**ให้คลิก**การปฏิบัติตามกฎระเบียบอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="036dc-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="036dc-109">ดูรายงานการปฏิบัติตามกฎระเบียบของอุปกรณ์เพื่อตรวจสอบว่า อุปกรณ์ของผู้ใช้ถูกทำเครื่องหมายเป็นไปตามข้อกำหนด</span><span class="sxs-lookup"><span data-stu-id="036dc-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="036dc-110">ในเว็บไซต์ Azure ไป**Intune\>ปฏิบัติตามกฎระเบียบอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="036dc-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="036dc-111">ภายใต้การ**จัดการ**คลิก**นโยบาย**</span><span class="sxs-lookup"><span data-stu-id="036dc-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="036dc-112">ในรายการของนโยบายการปฏิบัติตามกฎระเบียบ ตรวจสอบว่า มีกำหนดโพรไฟล์กับอุปกรณ์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="036dc-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="036dc-113">ถ้ามีกำหนดโพรไฟล์ไม่มี แล้ว Intune จะไม่สามารถยืนยันสถานะการปฏิบัติตามกฎระเบียบของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="036dc-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="036dc-114">แก้ไขการมอบหมายแบบมีเงื่อนไขในการเข้าถึงของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="036dc-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="036dc-115">ในเว็บไซต์ Azure ไป**Intune\>เข้าตามเงื่อนไข\>นโยบาย**</span><span class="sxs-lookup"><span data-stu-id="036dc-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="036dc-116">เลือกนโยบายการเลือกจากรายการ</span><span class="sxs-lookup"><span data-stu-id="036dc-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="036dc-117">คลิก**ผู้ใช้และกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="036dc-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="036dc-118">เมื่อต้องการกำหนดเป้าหมายนโยบายที่บุคคลอื่น เพิ่มลงในรายการการ**รวม**</span><span class="sxs-lookup"><span data-stu-id="036dc-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="036dc-119">เพื่อให้แน่ใจว่า บุคคลที่ถูกตัดออกจากนโยบาย เพิ่มเข้าไปในรายการข้อ**ยกเว้น**</span><span class="sxs-lookup"><span data-stu-id="036dc-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="036dc-120">อ่านเพิ่มเติม:[วิธีการอุปกรณ์ตรวจสอบการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="036dc-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

