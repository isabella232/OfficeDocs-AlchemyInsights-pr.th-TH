---
title: ซิงค์กลุ่ม
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256915"
---
# <a name="group-sync"></a>ซิงค์กลุ่ม

บทความนี้มีแนวทางในการซิงโครไนซ์กลุ่ม

1. ถ้าผู้ดูแลระบบส่วนกลางหรือเจ้าของกลุ่มไม่สามารถปรับเปลี่ยนคุณสมบัติกลุ่ม หรือเพิ่มสมาชิก หรือกําหนดเจ้าของในพอร์ทัล Azure ตรวจสอบให้แน่ใจว่าแหล่งข้อมูลของผู้ให้บริการออกของกลุ่มคือ Azure Active Directory (Azure AD) ให้กับผู้ดูแลระบบส่วนกลางหรือเจ้าของกลุ่มเพื่อปรับเปลี่ยนกลุ่ม
2. ก่อนที่จะพยายามลบกลุ่มที่ซิงค์ใน Azure AD ตรวจสอบให้แน่ใจว่าคุณได้ [ลบสิทธิ์การใช้งานที่ได้รับมอบหมายทั้งหมด](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) เพื่อหลีกเลี่ยงข้อผิดพลาด

เพื่อความเข้าใจเกี่ยวกับวิธีการซิงค์ผู้ใช้ กลุ่ม และที่ติดต่อ ให้ดู [การซิงค์ Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)และติดตามการซิงค์กลุ่มภายในองค์กรกับ Azure โดยใช้ [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) เพื่อซิงค์กลุ่มภายในองค์กรโดยใช้ AD Connect

ให้ปฏิบัติตามคู่มือ [นี้ การแก้ไขปัญหาข้อผิดพลาดระหว่างการ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) ซิงโครไนซ์เพื่อแก้ไขข้อผิดพลาดทั่วไประหว่างการซิงโครไนซ์

