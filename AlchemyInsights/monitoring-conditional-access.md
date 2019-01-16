---
title: ตรวจสอบการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317185"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="52281-102">ตรวจสอบการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="52281-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="52281-p101">ผู้ใช้ที่เป็นเป้าหมาย มีการเข้าถึงแบบมีเงื่อนไขจะได้รับอีเมลการแจ้งเตือนถ้าพวกเขาไม่ตรงกับความต้องการเข้าถึงขององค์กรของคุณ เมื่อต้องการแก้ไข เราขอแนะนำการแก้ไขปัญหาต่อไปนี้อย่างใดอย่างหนึ่ง:</span><span class="sxs-lookup"><span data-stu-id="52281-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="52281-p102">ถ้าอุปกรณ์เป็น presumed เมื่อต้องการลงทะเบียน คำแนะนำผู้ใช้ไปยังแอพลิเคชันเว็บไซต์บริษัท และตรวจสอบว่า จะปรากฏอยู่ในเว็บไซต์บริษัท หากโปรแกรมไม่ ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="52281-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="52281-p103">ในเว็บไซต์ Azure ไป**Intune\>ปฏิบัติตามกฎระเบียบอุปกรณ์** ภายใต้**จอภาพ**ให้คลิก**การปฏิบัติตามกฎระเบียบอุปกรณ์** ดูรายงานการปฏิบัติตามกฎระเบียบของอุปกรณ์เพื่อตรวจสอบว่า อุปกรณ์ของผู้ใช้ถูกทำเครื่องหมายเป็นไปตามข้อกำหนด</span><span class="sxs-lookup"><span data-stu-id="52281-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="52281-p104">ในเว็บไซต์ Azure ไป**Intune\>ปฏิบัติตามกฎระเบียบอุปกรณ์** ภายใต้การ**จัดการ**คลิก**นโยบาย** ในรายการของนโยบายการปฏิบัติตามกฎระเบียบ ตรวจสอบว่า มีกำหนดโพรไฟล์กับอุปกรณ์ของผู้ใช้ ถ้ามีกำหนดโพรไฟล์ไม่มี แล้ว Intune จะไม่สามารถยืนยันสถานะการปฏิบัติตามกฎระเบียบของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="52281-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="52281-114">แก้ไขการมอบหมายแบบมีเงื่อนไขในการเข้าถึงของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="52281-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="52281-115">ในเว็บไซต์ Azure ไป**Intune\>เข้าตามเงื่อนไข\>นโยบาย**</span><span class="sxs-lookup"><span data-stu-id="52281-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="52281-116">เลือกนโยบายการเลือกจากรายการ</span><span class="sxs-lookup"><span data-stu-id="52281-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="52281-117">คลิก**ผู้ใช้และกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="52281-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="52281-p105">เมื่อต้องการกำหนดเป้าหมายนโยบายที่บุคคลอื่น เพิ่มลงในรายการการ**รวม** เพื่อให้แน่ใจว่า บุคคลที่ถูกตัดออกจากนโยบาย เพิ่มเข้าไปในรายการข้อ**ยกเว้น**</span><span class="sxs-lookup"><span data-stu-id="52281-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="52281-120">อ่านเพิ่มเติม:[วิธีการอุปกรณ์ตรวจสอบการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="52281-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

