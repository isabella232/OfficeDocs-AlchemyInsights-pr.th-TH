---
title: เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่าย
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494546"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="59a98-102">เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่ายได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="59a98-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="59a98-103">เพิ่มผู้ติดต่อภายนอกเพื่อกลุ่มแบบการกระจายสินค้า (DG) เป็นกระบวนการขั้นตอนที่ 2:</span><span class="sxs-lookup"><span data-stu-id="59a98-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="59a98-104">สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:</span><span class="sxs-lookup"><span data-stu-id="59a98-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="59a98-105">ในศูนย์ดูแล ไปที่**ผู้ใช้** > หน้าบุคคลที่[ติดต่อ](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="59a98-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="59a98-106">เลือก**เพิ่มผู้ติดต่อ**</span><span class="sxs-lookup"><span data-stu-id="59a98-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="59a98-107">พิมพ์ข้อมูลสำหรับผู้ติดต่อของคุณ และเลือก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="59a98-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="59a98-108">เพิ่มติดต่อจดหมาย DG ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="59a98-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="59a98-109">ในศูนย์ดูแล ไปที่**กลุ่ม** > [กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)หน้า</span><span class="sxs-lookup"><span data-stu-id="59a98-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="59a98-110">พบ DG คุณต้องการเพิ่มผู้ใช้ภายนอก และเลือกเพื่อเปิดกล่องโต้ตอบการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="59a98-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="59a98-111">บนแท็บ**สมาชิก**เลือก**ดูทั้งหมด และจัดการสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="59a98-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="59a98-112">เลือกการ**เพิ่มสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="59a98-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="59a98-113">เลือกผู้ติดต่อจดหมายคุณสร้างในขั้นตอนก่อนหน้า จากนั้น**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="59a98-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="59a98-114">ถ้าหลังจากทำตามขั้นตอนเหล่านี้ ของผู้ใช้ภายนอกไม่สามารถส่งอีเมล์ไป DG หรือไม่ได้รับอีเมลจากนั้น อาจว่า DG ที่ถูกทำเครื่องหมายเพื่ออนุญาตให้อีเมล์จากผู้ใช้ภายในเท่า นั้น</span><span class="sxs-lookup"><span data-stu-id="59a98-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="59a98-115">คุณสามารถตรวจสอบการตั้งค่าคอนฟิกนี้ และแก้ไขปัญหาให้ทำตามคำแนะนำ[ที่นี่](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)ได้</span><span class="sxs-lookup"><span data-stu-id="59a98-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="59a98-116">**หมายเหตุ:** คำแนะนำเหล่านี้ไม่สามารถใช้กับถ้าชนิดของกลุ่ม "Office 365 กลุ่ม" แทนที่เป็น "กลุ่มการแจกจ่าย"</span><span class="sxs-lookup"><span data-stu-id="59a98-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="59a98-117">ถ้าเป็นกรณีนี้ คุณสามารถเพิ่มผู้ใช้ภายนอกให้กับกลุ่มได้โดยตรงจาก Outlook</span><span class="sxs-lookup"><span data-stu-id="59a98-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="59a98-118">รายละเอียดเกี่ยวกับ Office 365 กลุ่มแขกเช่นเดียวกับคำแนะนำสำหรับการเพิ่มแขกภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="59a98-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  