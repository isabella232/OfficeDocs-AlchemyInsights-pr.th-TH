---
title: การกำหนดกลุ่มให้กับบทบาท Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885400"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="e9131-102">การกำหนดกลุ่มให้กับบทบาท Azure AD</span><span class="sxs-lookup"><span data-stu-id="e9131-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="e9131-103">เมื่อต้องการกำหนดกลุ่ม AD Azure ที่มีแหล่งที่มาของหน่วยงานใน Azure AD ไปยังบทบาท AD Azure ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e9131-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="e9131-104">สร้างกลุ่มใหม่-เมื่อต้องการสร้างกลุ่มใหม่ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="e9131-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="e9131-105">a.</span><span class="sxs-lookup"><span data-stu-id="e9131-105">a.</span></span> <span data-ttu-id="e9131-106">ลงชื่อเข้าใช้ศูนย์การจัดการ Azure AD ด้วย **ผู้ดูแลระบบบทบาทพิเศษ** หรือสิทธิ์ **ผู้ดูแลระบบส่วนกลาง**</span><span class="sxs-lookup"><span data-stu-id="e9131-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="e9131-107">b.</span><span class="sxs-lookup"><span data-stu-id="e9131-107">b.</span></span> <span data-ttu-id="e9131-108">เลือก **กลุ่ม > Azure Active directory > กลุ่มทั้งหมด > กลุ่มใหม่**</span><span class="sxs-lookup"><span data-stu-id="e9131-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="e9131-109">c.</span><span class="sxs-lookup"><span data-stu-id="e9131-109">c.</span></span> <span data-ttu-id="e9131-110">สร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="e9131-110">Create the group.</span></span>

2. <span data-ttu-id="e9131-111">กำหนดบทบาทให้กับกลุ่มทั้งในระหว่างการสร้างกลุ่มหรือหลังจากสร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="e9131-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="e9131-112">a.</span><span class="sxs-lookup"><span data-stu-id="e9131-112">a.</span></span> <span data-ttu-id="e9131-113">เมื่อต้องการกำหนดบทบาทให้กับกลุ่มในช่วงเวลาของการสร้างกลุ่มให้สลับไปยัง **บทบาทสลับ AZURE AD ที่สามารถกำหนดให้กับกลุ่ม** และสร้างกลุ่มได้</span><span class="sxs-lookup"><span data-stu-id="e9131-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="e9131-114">b.</span><span class="sxs-lookup"><span data-stu-id="e9131-114">b.</span></span> <span data-ttu-id="e9131-115">เมื่อต้องการกำหนดบทบาทให้กับกลุ่มหลังจากที่สร้างขึ้นแล้วให้นำทางไปยังแท็บ **บทบาทที่มอบหมาย** สำหรับกลุ่มที่สร้างขึ้นใหม่และกำหนดบทบาทให้กับกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="e9131-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="e9131-116">**จัดการการเป็นสมาชิกของกลุ่มที่กำหนดให้กับบทบาท Azure AD**</span><span class="sxs-lookup"><span data-stu-id="e9131-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="e9131-117">เมื่อต้องการป้องกันไม่ให้มีสิทธิ์การใช้งานตามค่าเริ่มต้นเฉพาะผู้ดูแลระบบบทบาทที่มีสิทธิ์และผู้ดูแลระบบส่วนกลางเท่านั้นที่สามารถปรับเปลี่ยนการเป็นสมาชิกของกลุ่มที่ถูกกำหนดให้กับบทบาทได้</span><span class="sxs-lookup"><span data-stu-id="e9131-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="e9131-118">อย่างไรก็ตามพวกเขาสามารถเลือกที่จะกำหนดเจ้าของให้กับกลุ่มดังกล่าวและมอบหมายงานนี้</span><span class="sxs-lookup"><span data-stu-id="e9131-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="e9131-119">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการกำหนดกลุ่ม cloud ให้กับบทบาท Azure AD ให้ดู[ที่กำหนดบทบาทโฆษณาให้กับกลุ่ม cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)</span><span class="sxs-lookup"><span data-stu-id="e9131-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="e9131-120">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาบทบาทที่มอบหมายให้กับกลุ่ม cloud ให้ดูที่การ[แก้ไขปัญหาบทบาทที่มอบหมายให้กับกลุ่ม cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="e9131-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





