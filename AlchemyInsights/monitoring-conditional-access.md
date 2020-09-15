---
title: การตรวจสอบการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702922"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0ec5f-102">การตรวจสอบการเข้าถึงแบบมีเงื่อนไขสำหรับ Exchange</span><span class="sxs-lookup"><span data-stu-id="0ec5f-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0ec5f-103">ผู้ใช้ที่กำหนดเป้าหมายด้วยการเข้าถึงแบบมีเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ตรงตามข้อกำหนดของการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="0ec5f-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0ec5f-104">เมื่อต้องการแก้ไขเราขอแนะนำวิธีแก้ไขปัญหาอย่างน้อยหนึ่งอย่างต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0ec5f-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0ec5f-105">ถ้ามีการลงทะเบียนอุปกรณ์ให้ให้คำแนะนำให้ผู้ใช้ไปที่แอป Portal ของบริษัทและตรวจสอบว่าปรากฏในพอร์ทัลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="0ec5f-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0ec5f-106">ถ้าไม่ใช่ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="0ec5f-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0ec5f-107">ในพอร์ทัล Azure ให้ไปที่ **การ \> ปฏิบัติตาม**ข้อกำหนดของอุปกรณ์ Intune</span><span class="sxs-lookup"><span data-stu-id="0ec5f-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0ec5f-108">ภายใต้การ **ตรวจสอบ** ให้คลิกการ **ปฏิบัติตาม**ข้อกำหนดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="0ec5f-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="0ec5f-109">ดูรายงานการปฏิบัติตามนโยบายของอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้ได้รับการทำเครื่องหมายว่าสอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="0ec5f-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0ec5f-110">ในพอร์ทัล Azure ให้ไปที่ **การ \> ปฏิบัติตาม**ข้อกำหนดของอุปกรณ์ Intune</span><span class="sxs-lookup"><span data-stu-id="0ec5f-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0ec5f-111">ภายใต้**จัดการ**ให้คลิก**นโยบาย**</span><span class="sxs-lookup"><span data-stu-id="0ec5f-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="0ec5f-112">ในรายการนโยบายการปฏิบัติตามนโยบายให้ตรวจสอบว่าโปรไฟล์ถูกกำหนดให้กับอุปกรณ์ของผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="0ec5f-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0ec5f-113">ถ้าไม่มีการกำหนดโปรไฟล์จากนั้น Intune จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="0ec5f-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0ec5f-114">แก้ไขการกำหนดสิทธิ์การเข้าถึงตามเงื่อนไขของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="0ec5f-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0ec5f-115">ในพอร์ทัล Azure ไปที่\*\*นโยบายการ \> เข้าถึง \> \*\*แบบมีเงื่อนไขของ Intune</span><span class="sxs-lookup"><span data-stu-id="0ec5f-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0ec5f-116">เลือกนโยบายจากรายการ</span><span class="sxs-lookup"><span data-stu-id="0ec5f-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0ec5f-117">คลิก **ผู้ใช้และกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="0ec5f-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0ec5f-118">เมื่อต้องการกำหนดเป้าหมายให้กับนโยบายบางอย่างที่มีใครบางคนให้เพิ่มลงในรายการ**รวม**</span><span class="sxs-lookup"><span data-stu-id="0ec5f-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="0ec5f-119">เมื่อต้องการตรวจสอบให้แน่ใจว่าบุคคลถูกละเว้นจากนโยบายให้เพิ่มลงในรายการที่**แยก**</span><span class="sxs-lookup"><span data-stu-id="0ec5f-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0ec5f-120">อ่านเพิ่มเติม:[วิธีการตรวจสอบอุปกรณ์การเข้าถึง](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)แบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="0ec5f-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

