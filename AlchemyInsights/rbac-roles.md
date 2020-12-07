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
# <a name="rbac-rules"></a>กฎ RBAC

ถ้าคุณได้รับข้อผิดพลาดสิทธิ์: 

- **ไคลเอ็นต์ที่มี id ของวัตถุไม่ได้รับอนุญาตให้ดำเนินการผ่านขอบเขต (โค้ด: AuthorizationFailed)**: เมื่อคุณพยายามสร้างทรัพยากรให้ตรวจสอบว่าคุณได้ลงชื่อเข้าใช้ด้วยผู้ใช้ที่ได้รับมอบหมายบทบาทที่มีสิทธิ์ในการเขียนไปยังทรัพยากรที่ขอบเขตที่เลือก ตัวอย่างเช่นเมื่อต้องการจัดการเครื่องเสมือนในกลุ่มทรัพยากรคุณควรมีบทบาทผู้ [สนับสนุนเครื่องเสมือน](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) บนกลุ่มทรัพยากร (หรือขอบเขตหลัก) สำหรับรายการสิทธิ์สำหรับบทบาทที่มีอยู่แล้วภายในให้ดู[ที่บทบาทที่มีอยู่แล้วภายในสำหรับทรัพยากร Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- **คุณไม่มีสิทธิ์ในการสร้างคำขอการสนับสนุน**: เมื่อคุณพยายามสร้างหรืออัปเดตการสนับสนุนตั๋วให้ตรวจสอบว่าคุณได้ลงชื่อเข้าใช้ด้วยผู้ใช้ที่ได้รับการกำหนดบทบาทที่มีสิทธิ์ในการสนับสนุน/supportTickets/เขียนเช่นการ [สนับสนุนการร้องขอ](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)การสนับสนุน
- **ไม่สามารถสร้างงานที่มอบหมายบทบาทเพิ่มเติมได้ (รหัส: RoleAssignmentLimitExceeded)**: เมื่อคุณพยายามที่จะกำหนดบทบาทให้ลองลดจำนวนของงานที่มอบหมายบทบาทโดยการกำหนดบทบาทให้กับกลุ่มแทน Azure สนับสนุนการมอบหมายบทบาทของ **๒๐๐๐** ต่อการสมัครใช้งาน

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับบทบาทของ Azure RBAC ให้ดูที่[บทบาทของ AZURE rbac](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
