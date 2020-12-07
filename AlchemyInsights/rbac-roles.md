---
title: 'บทบาท RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583955"
---
# <a name="rbac-rules"></a><span data-ttu-id="94785-102">กฎ RBAC</span><span class="sxs-lookup"><span data-stu-id="94785-102">RBAC rules</span></span>

<span data-ttu-id="94785-103">ถ้าคุณได้รับข้อผิดพลาดสิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="94785-103">If you get the permission error:</span></span> 

- <span data-ttu-id="94785-104">**ไคลเอ็นต์ที่มี id ของวัตถุไม่ได้รับอนุญาตให้ดำเนินการผ่านขอบเขต (โค้ด: AuthorizationFailed)**: เมื่อคุณพยายามสร้างทรัพยากรให้ตรวจสอบว่าคุณได้ลงชื่อเข้าใช้ด้วยผู้ใช้ที่ได้รับมอบหมายบทบาทที่มีสิทธิ์ในการเขียนไปยังทรัพยากรที่ขอบเขตที่เลือก</span><span class="sxs-lookup"><span data-stu-id="94785-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="94785-105">ตัวอย่างเช่นเมื่อต้องการจัดการเครื่องเสมือนในกลุ่มทรัพยากรคุณควรมีบทบาทผู้ [สนับสนุนเครื่องเสมือน](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) บนกลุ่มทรัพยากร (หรือขอบเขตหลัก)</span><span class="sxs-lookup"><span data-stu-id="94785-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="94785-106">สำหรับรายการสิทธิ์สำหรับบทบาทที่มีอยู่แล้วภายในให้ดู[ที่บทบาทที่มีอยู่แล้วภายในสำหรับทรัพยากร Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="94785-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="94785-107">**คุณไม่มีสิทธิ์ในการสร้างคำขอการสนับสนุน**: เมื่อคุณพยายามสร้างหรืออัปเดตการสนับสนุนตั๋วให้ตรวจสอบว่าคุณได้ลงชื่อเข้าใช้ด้วยผู้ใช้ที่ได้รับการกำหนดบทบาทที่มีสิทธิ์ในการสนับสนุน/supportTickets/เขียนเช่นการ [สนับสนุนการร้องขอ](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)การสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="94785-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="94785-108">**ไม่สามารถสร้างงานที่มอบหมายบทบาทเพิ่มเติมได้ (รหัส: RoleAssignmentLimitExceeded)**: เมื่อคุณพยายามที่จะกำหนดบทบาทให้ลองลดจำนวนของงานที่มอบหมายบทบาทโดยการกำหนดบทบาทให้กับกลุ่มแทน</span><span class="sxs-lookup"><span data-stu-id="94785-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="94785-109">Azure สนับสนุนการมอบหมายบทบาทของ **๒๐๐๐** ต่อการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="94785-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="94785-110">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับบทบาทของ Azure RBAC ให้ดูที่[บทบาทของ AZURE rbac](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="94785-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
