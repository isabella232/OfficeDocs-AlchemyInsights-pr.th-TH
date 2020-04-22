---
title: การตรวจสอบการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713737"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="f21f4-102">การตรวจสอบการเข้าถึงแบบมีเงื่อนไขสําหรับการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="f21f4-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="f21f4-103">ผู้ใช้ที่กําหนดเป้าหมายด้วยการเข้าถึงแบบมีเงื่อนไขจะได้รับอีเมลการแจ้งเตือนหากผู้ใช้ไม่เป็นไปตามข้อกําหนดการเข้าถึงขององค์กร</span><span class="sxs-lookup"><span data-stu-id="f21f4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f21f4-104">เมื่อต้องการแก้ไข เราขอแนะนําอย่างน้อยหนึ่งวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f21f4-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="f21f4-105">หากอุปกรณ์ถูกสันนิษฐานให้ลงทะเบียน ให้แนะนําผู้ใช้ให้ไปยังแอปพอร์ทัลของบริษัท และตรวจสอบว่าอุปกรณ์นั้นปรากฏในพอร์ทัลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="f21f4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f21f4-106">หากไม่ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="f21f4-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="f21f4-107">ในพอร์ทัล Azure ไปที่**การปฏิบัติตามข้อกําหนด\>ของอุปกรณ์ Intune**</span><span class="sxs-lookup"><span data-stu-id="f21f4-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f21f4-108">ภายใต้**ตรวจสอบ**คลิก**การปฏิบัติตามอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="f21f4-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="f21f4-109">ดูรายงานการปฏิบัติตามอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้ถูกทําเครื่องหมายว่าเป็นไปตามข้อกําหนดหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f21f4-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="f21f4-110">ในพอร์ทัล Azure ไปที่**การปฏิบัติตามข้อกําหนด\>ของอุปกรณ์ Intune**</span><span class="sxs-lookup"><span data-stu-id="f21f4-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f21f4-111">ภายใต้**จัดการ**ให้คลิก**นโยบาย**</span><span class="sxs-lookup"><span data-stu-id="f21f4-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="f21f4-112">ในรายการนโยบายการปฏิบัติตามกฎระเบียบ ให้ตรวจสอบว่าโปรไฟล์ถูกกําหนดให้กับอุปกรณ์ของผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f21f4-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f21f4-113">ถ้าไม่มีการกําหนดโปรไฟล์ Intune จะไม่สามารถยืนยันสถานะการปฏิบัติตามของอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="f21f4-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="f21f4-114">แก้ไขการกําหนดการเข้าถึงแบบมีเงื่อนไขของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f21f4-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="f21f4-115">ในพอร์ทัล Azure ไปที่**นโยบายการเข้าถึง\>\>แบบมีเงื่อนไขของ Intune**</span><span class="sxs-lookup"><span data-stu-id="f21f4-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="f21f4-116">เลือกนโยบายจากรายการ</span><span class="sxs-lookup"><span data-stu-id="f21f4-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="f21f4-117">คลิก**ผู้ใช้และกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="f21f4-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="f21f4-118">หากต้องการกําหนดเป้าหมายนโยบายบางนโยบายที่บางคน ให้เพิ่มนโยบายเหล่านั้นลงในรายการ**รวม**</span><span class="sxs-lookup"><span data-stu-id="f21f4-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="f21f4-119">เมื่อต้องการให้บุคคลถูกละเว้นจากนโยบาย ให้เพิ่มบุคคลเหล่านั้นลงในรายการ**ยกเว้น**</span><span class="sxs-lookup"><span data-stu-id="f21f4-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="f21f4-120">อ่านเพิ่มเติม:[วิธีการตรวจสอบอุปกรณ์การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="f21f4-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

