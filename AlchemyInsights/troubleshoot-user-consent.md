---
title: การแก้ไขปัญหาความยินยอมของผู้ใช้
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901627"
---
# <a name="troubleshoot-user-consent"></a>การแก้ไขปัญหาความยินยอมของผู้ใช้

1. คุณสามารถกำหนดค่าความยินยอมของผู้ใช้ไปยังแอปพลิเคชันผ่านทางพอร์ทัล Azure หรือ PowerShell ได้ สำหรับข้อมูลเพิ่มเติมให้ดูที่[การตั้งค่าความยินยอมของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)
1. ผู้ดูแลระบบยังสามารถใช้ API ของ [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) เพื่อให้ความยินยอมในการมอบสิทธิ์ในนามของผู้ใช้คนเดียวได้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่รับสิทธิ์การเข้าถึงในนามของผู้ใช้](https://docs.microsoft.com/graph/auth-v2-user)
1. [ข้อผิดพลาดในการยินยอมของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): บทความนี้จะอธิบายข้อผิดพลาดที่อาจเกิดขึ้นในระหว่างกระบวนการยินยอมให้กับแอปพลิเคชัน ถ้าคุณกำลังแก้ไขปัญหาพร้อมท์การยินยอมที่ไม่คาดคิดที่ไม่มีข้อความแสดงข้อผิดพลาดให้ดูที่[สถานการณ์การรับรองความถูกต้องสำหรับ AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)