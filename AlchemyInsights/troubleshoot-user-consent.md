---
title: แก้ไขปัญหาความยินยอมของผู้ใช้
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007917"
---
# <a name="troubleshoot-user-consent"></a>แก้ไขปัญหาความยินยอมของผู้ใช้

1. คุณสามารถกําหนดค่าวิธีการที่ผู้ใช้ยินยอมให้แอปพลิเคชันผ่านพอร์ทัล Azure หรือ PowerShell ดู [การตั้งค่าความยินยอมของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) เพื่อดูข้อมูลเพิ่มเติม
1. ผู้ดูแลระบบยังสามารถใช้ Microsoft [Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)ในการให้ความยินยอมกับสิทธิ์ที่ได้รับมอบหมายในนามของผู้ใช้รายเดียว For more information, [see Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).
1. [ข้อผิดพลาดการยินยอม](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)จากผู้ใช้: บทความนี้จะอธิบายถึงข้อผิดพลาดที่อาจเกิดขึ้นระหว่างกระบวนการยินยอมให้แอปพลิเคชัน ถ้าคุณแก้ไขปัญหาพร้อมท์การยินยอมที่ไม่คาดคิดที่ไม่มีข้อความแสดงข้อผิดพลาด ให้ดู สถานการณ์[การรับรองความถูกต้องของ Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)