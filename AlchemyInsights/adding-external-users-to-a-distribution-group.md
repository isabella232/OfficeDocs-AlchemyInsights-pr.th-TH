---
title: เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่าย
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660811"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="b1d4e-102">เพิ่มผู้ใช้ภายนอกไปยัง กลุ่มการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="b1d4e-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="b1d4e-103">เพิ่มผู้ติดต่อภายนอกเพื่อกลุ่มแบบการกระจายสินค้า (DG) เป็นกระบวนการสองขั้นตอน:</span><span class="sxs-lookup"><span data-stu-id="b1d4e-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="b1d4e-104">สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:</span><span class="sxs-lookup"><span data-stu-id="b1d4e-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="b1d4e-105">ในศูนย์ดูแล ไปที่**ผู้ใช้** > หน้าบุคคลที่[ติดต่อ](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="b1d4e-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="b1d4e-106">เลือก**เพิ่มผู้ติดต่อ**</span><span class="sxs-lookup"><span data-stu-id="b1d4e-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="b1d4e-107">พิมพ์ข้อมูลสำหรับผู้ติดต่อของคุณ และเลือก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="b1d4e-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="b1d4e-108">เพิ่มติดต่อจดหมาย DG ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b1d4e-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="b1d4e-109">ในศูนย์ดูแล ไปที่**กลุ่ม** > [กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)หน้า</span><span class="sxs-lookup"><span data-stu-id="b1d4e-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="b1d4e-110">พบ DG คุณต้องการเพิ่มผู้ใช้ภายนอก และเลือกเพื่อเปิดกล่องโต้ตอบการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="b1d4e-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="b1d4e-111">บนแท็บ**สมาชิก**เลือก**ดูทั้งหมด และจัดการสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="b1d4e-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="b1d4e-112">เลือกการ**เพิ่มสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="b1d4e-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="b1d4e-113">เลือกผู้ติดต่อจดหมายคุณสร้างในขั้นตอนก่อนหน้า จากนั้น**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b1d4e-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="b1d4e-114">ถ้าหลังจากทำตามขั้นตอนเหล่านี้ ของผู้ใช้ภายนอกไม่สามารถส่งอีเมล์ไป DG หรือไม่ได้รับอีเมลจากนั้น อาจว่า DG ที่ถูกทำเครื่องหมายเพื่ออนุญาตให้อีเมล์จากผู้ใช้ภายในเท่า นั้น</span><span class="sxs-lookup"><span data-stu-id="b1d4e-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="b1d4e-115">คุณสามารถตรวจสอบการตั้งค่าคอนฟิกนี้ และแก้ไขปัญหาให้ทำตามคำแนะนำ[ที่นี่](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)ได้</span><span class="sxs-lookup"><span data-stu-id="b1d4e-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="b1d4e-116">**หมายเหตุ:** คำแนะนำเหล่านี้ไม่สามารถใช้กับถ้าชนิดของกลุ่ม "Office 365 กลุ่ม" แทนที่เป็น "กลุ่มการแจกจ่าย"</span><span class="sxs-lookup"><span data-stu-id="b1d4e-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="b1d4e-117">ถ้าเป็นกรณีนี้ คุณสามารถเพิ่มผู้ใช้ภายนอกให้กับกลุ่มได้โดยตรงจาก Outlook</span><span class="sxs-lookup"><span data-stu-id="b1d4e-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="b1d4e-118">รายละเอียดเกี่ยวกับ Office 365 กลุ่มแขกเช่นเดียวกับคำแนะนำสำหรับการเพิ่มแขกภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="b1d4e-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  