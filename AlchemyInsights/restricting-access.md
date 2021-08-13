---
title: การจํากัดการเข้าถึง
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7769"
ms.openlocfilehash: 98057b8e34cad19e2118f470dbeacdc8a7e78d9bc941e7f6565743201a541b56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958676"
---
# <a name="restricting-access"></a>การจํากัดการเข้าถึง

1. For information on how to restrict access to an application, see [How to: Restrict your Azure AD app to a set of users in an Azure AD tenant](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users).
1. เรียนรู้วิธีการตรวจทานและจัดการสิทธิ์ของแอปพลิเคชัน [ใช้การกระทั่งกับแอปพลิเคชันที่สมัครใช้งานเกิน](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application)หรือน่าสงสัยใน Azure Active Directory ให้การกระทั่งต่างๆ ที่คุณสามารถกระทั่งการรักษาความปลอดภัยแอปพลิเคชันของคุณตามสถานการณ์ การตกลงเหล่านี้จะใช้กับแอปพลิเคชันทั้งหมดที่ถูกเพิ่มลงในผู้เช่า Azure Active Directoryของคุณ (Azure AD) ผ่านความยินยอมของผู้ใช้หรือผู้ดูแลระบบ
1. [จัดการการมอบหมายผู้ใช้ของแอปใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment)จะแสดงวิธีการกําหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันขององค์กรใน Azure Active Directory (Azure AD) จากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell เมื่อคุณกําหนดให้ผู้ใช้ไปยังแอปพลิเคชัน แอปพลิเคชันจะปรากฏในแอปของฉันของผู้ใช้เพื่อให้เข้าถึงได้ง่าย ถ้าแอปพลิเคชันแสดงบทบาท คุณยังสามารถกําหนดบทบาทเฉพาะให้กับผู้ใช้ได้
    - For more information on User and Group assignment see [Conditional Access: Users and groups](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups).
