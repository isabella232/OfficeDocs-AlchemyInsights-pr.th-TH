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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923150"
---
# <a name="rbac-rules"></a>กฎ RBAC

ถ้าคุณได้รับข้อผิดพลาดสิทธิ์: 

- ไคลเอ็นต์ที่มี ID วัตถุไม่มีสิทธิ์ในการปฏิบัติเกินขอบเขต **(โค้ด: AuthorizationFailed)**: เมื่อคุณพยายามสร้างทรัพยากร ให้ตรวจสอบว่าคุณได้ลงชื่อเข้าใช้กับผู้ใช้ที่ได้รับมอบหมายบทบาทที่มีสิทธิ์เขียนไปยังทรัพยากรที่ขอบเขตที่เลือก ตัวอย่างเช่น เมื่อต้องการจัดการเครื่องเสมือนในกลุ่มทรัพยากร คุณควรมีบทบาท Virtual Machine [Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) บนกลุ่มทรัพยากร (หรือขอบเขตแม่) For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- คุณไม่มีสิทธิ์ในการสร้างการร้องขอการสนับสนุน **:** เมื่อคุณพยายามสร้างหรืออัปเดตตั๋วการสนับสนุน ตรวจสอบว่าคุณลงชื่อเข้าใช้กับผู้ใช้ที่ได้รับมอบหมายบทบาทที่มีสิทธิ์ Microsoft.Support/supportTickets/write อยู่ เช่น [ผู้สนับสนุน](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)ขอรับการสนับสนุน
- **คุณสามารถสร้างการมอบหมายบทบาทได้ไม่เกิน (โค้ด: RoleAssignmentLimitExceeded)**: เมื่อคุณพยายามกําหนดบทบาท ลองลดจํานวนการมอบหมายบทบาทโดยการกําหนดบทบาทให้กับกลุ่มแทน Azure สนับสนุนการมอบหมาย **บทบาทสูงสุด 2,000** คนต่อการสมัครใช้งาน

For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
