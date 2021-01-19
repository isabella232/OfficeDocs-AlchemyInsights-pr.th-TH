---
title: สิทธิ์ในการให้สิทธิ์
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
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901618"
---
# <a name="grant-permissions"></a>สิทธิ์ในการให้สิทธิ์

1. ให้ความยินยอมในการ **จัดการผู้เช่า**: ดูให้ความยินยอมจาก [ผู้ดูแลระบบสำหรับผู้เช่า](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)สำหรับคำแนะนำทีละขั้นตอนสำหรับคำแนะนำทีละขั้นตอนสำหรับการให้ความยินยอมจากผู้เช่าที่ได้รับอนุญาตจากพอร์ทัล AZURE โดยใช้ PowerShell AD azure หรือจากพร้อมท์ความยินยอมเอง
1. ให้ความ **ยินยอมในนามของผู้ใช้ที่เฉพาะเจาะจง**: แทนที่จะให้ความยินยอมสำหรับทั้งองค์กรผู้ดูแลระบบยังสามารถใช้ [API Microsoft Graph](https://docs.microsoft.com/graph/use-the-api)เพื่อให้สิทธิ์ในการมอบสิทธิ์ในนามของผู้ใช้คนเดียวได้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่รับสิทธิ์การเข้าถึงในนามของผู้ใช้](https://docs.microsoft.com/graph/auth-v2-user)