---
title: เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่ายหรือไม่
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398477"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="23e69-102">เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่ายหรือไม่</span><span class="sxs-lookup"><span data-stu-id="23e69-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="23e69-103">เพิ่มผู้ติดต่อภายนอกเพื่อกลุ่มแบบการกระจายสินค้า (DG) เป็นกระบวนการขั้นตอนที่ 2:</span><span class="sxs-lookup"><span data-stu-id="23e69-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="23e69-104">สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:</span><span class="sxs-lookup"><span data-stu-id="23e69-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="23e69-105">คลิกที่[นี่](https://admin.microsoft.com/adminportal/home#/Contact)เพื่อไปยังหน้าแก้ไขผู้ติดต่อใน Admin เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="23e69-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="23e69-106">คลิกที่**เพิ่มผู้ติดต่อ**</span><span class="sxs-lookup"><span data-stu-id="23e69-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="23e69-107">พิมพ์ข้อมูลสำหรับผู้ติดต่อของคุณ และคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="23e69-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="23e69-108">เพิ่มติดต่อจดหมาย DG ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="23e69-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="23e69-109">คลิกที่[นี่](https://admin.microsoft.com/adminportal/home#/groups)เพื่อไปยังหน้ากลุ่ม</span><span class="sxs-lookup"><span data-stu-id="23e69-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="23e69-110">พบ DG คุณต้องการเพิ่มผู้ใช้ภายนอก และคลิกบนวัตถุเพื่อเปิดกล่องโต้ตอบการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="23e69-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="23e69-111">คลิกที่ปุ่ม**แก้ไข**ในรายการ**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="23e69-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="23e69-112">คลิกที่**เพิ่มสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="23e69-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="23e69-113">เลือกผู้ติดต่อจดหมายคุณสร้างในขั้นตอนก่อนหน้านี้ และคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="23e69-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="23e69-114">แม้หลังจากทำตามขั้นตอนเหล่านี้ ของผู้ใช้ภายนอกไม่สามารถส่งอีเมล์ไป DG หรือไม่รับอีเมล์จากนั้น สามารถว่า DG ที่ถูกทำเครื่องหมายเพื่ออนุญาตให้อีเมล์จากผู้ใช้ภายในเท่า นั้น</span><span class="sxs-lookup"><span data-stu-id="23e69-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="23e69-115">คุณสามารถตรวจสอบการตั้งค่าคอนฟิกนี้ และแก้ไขปัญหาให้ทำตามคำแนะนำ[ที่นี่](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span><span class="sxs-lookup"><span data-stu-id="23e69-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="23e69-116">**หมายเหตุ:** คำแนะนำเหล่านี้ไม่สามารถใช้กับถ้าชนิดของกลุ่ม "Office 365 กลุ่ม" แทนที่เป็น "กลุ่มการแจกจ่าย"</span><span class="sxs-lookup"><span data-stu-id="23e69-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="23e69-117">ถ้าเป็นกรณีนี้ คุณสามารถเพิ่มผู้ใช้ภายนอกให้กับกลุ่มได้โดยตรงจาก Outlook หรือ Outlook บนเว็บ</span><span class="sxs-lookup"><span data-stu-id="23e69-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="23e69-118">คำอธิบายโดยละเอียดใน O365 กลุ่มแขกเช่นเดียวกับคำแนะนำสำหรับการเพิ่มแขกภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="23e69-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

