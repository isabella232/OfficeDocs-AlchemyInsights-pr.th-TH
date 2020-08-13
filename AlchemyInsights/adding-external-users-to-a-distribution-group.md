---
title: การเพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910951"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="b376b-102">เพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="b376b-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="b376b-103">การเพิ่มที่ติดต่อภายนอกลงในกลุ่มการแจกจ่าย (DG) เป็นกระบวนการสองขั้นตอนดังนี้</span><span class="sxs-lookup"><span data-stu-id="b376b-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="b376b-104">สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:</span><span class="sxs-lookup"><span data-stu-id="b376b-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="b376b-105">ในศูนย์การจัดการให้ไปที่หน้าผู้ติดต่อของ**ผู้ใช้**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="b376b-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="b376b-106">เลือก**เพิ่มที่ติดต่อ**</span><span class="sxs-lookup"><span data-stu-id="b376b-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="b376b-107">พิมพ์ข้อมูลสำหรับที่ติดต่อของคุณแล้วเลือก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="b376b-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="b376b-108">เพิ่มที่ติดต่อจดหมายลงใน DG ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b376b-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="b376b-109">ในศูนย์การจัดการให้ไปที่หน้า**Groups**  >  [กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)กลุ่ม</span><span class="sxs-lookup"><span data-stu-id="b376b-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="b376b-110">ค้นหา DG ที่คุณต้องการเพิ่มผู้ใช้ภายนอกและเลือกกล่องโต้ตอบเพื่อเปิดกล่องโต้ตอบแก้ไข</span><span class="sxs-lookup"><span data-stu-id="b376b-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="b376b-111">บนแท็บ**สมาชิก**ให้เลือก**ดูทั้งหมดและจัดการสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="b376b-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="b376b-112">เลือก**เพิ่มสมาชิก**</span><span class="sxs-lookup"><span data-stu-id="b376b-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="b376b-113">เลือกที่ติดต่อจดหมายที่คุณสร้างขึ้นในขั้นตอนก่อนหน้านี้แล้วเลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b376b-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="b376b-114">ถ้าหลังจากทำตามขั้นตอนเหล่านี้ผู้ใช้ภายนอกของคุณไม่สามารถส่งอีเมลไปยัง DG หรือไม่ได้รับอีเมลจากอีเมลนั้นอาจเป็นไปได้ว่า DG ถูกทำเครื่องหมายให้อนุญาตอีเมลจากผู้ใช้ภายในเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="b376b-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="b376b-115">คุณสามารถตรวจสอบการกำหนดค่านี้และแก้ไขปัญหาตามคำแนะนำ[ที่นี่](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="b376b-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="b376b-116">**หมายเหตุ:** คำแนะนำเหล่านี้จะไม่นำไปใช้ถ้าชนิดของกลุ่มของคุณเป็น "Microsoft ๓๖๕ group" แทนที่จะเป็น "กลุ่มการแจกจ่าย"</span><span class="sxs-lookup"><span data-stu-id="b376b-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="b376b-117">ถ้าเป็นกรณีนี้คุณสามารถเพิ่มผู้ใช้ภายนอกลงในกลุ่มจาก Outlook ได้โดยตรง</span><span class="sxs-lookup"><span data-stu-id="b376b-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="b376b-118">ข้อมูลรายละเอียดเกี่ยวกับ Microsoft ๓๖๕กลุ่มผู้เข้าร่วมรวมถึงคำแนะนำสำหรับการเพิ่มผู้เยี่ยมชมภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="b376b-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  