---
title: แอปของฉันไม่แสดงขึ้นในการควบคุมแอป
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454988"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>แอปของฉันไม่แสดงขึ้นในการควบคุมแอป

ถ้าแอปพลิเคชันของคุณไม่แสดงขึ้นในการกํากับดูแลแอป ให้ตรวจสอบดังต่อไปนี้:

1. ไปที่ [Azure AD](https://aad.portal.azure.com/) และค้นหา ID แอปของแอปพลิเคชันของคุณโดยการค้นหาชื่อแอปในแถบด้านบนสุดบนหน้าภาพรวม

1. Access Graph Explorer และค้นหา ID ของแอปภายในหลักของบริการของคุณโดยใช้คิวรีนี้และแทนที่ด้วย ID ของแอปที่เกี่ยวข้อง <appId> : < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. ถ้าไม่มีผลลัพธ์ใดถูกส่งกลับ ให้ค้นหา ID ของแอปภายในแอปพลิเคชันโดยใช้คิวรีนี้ และแทนที่ด้วย ID ของแอปที่เกี่ยวข้อง <appId> : < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

ถ้าคุณพบปัญหาเกี่ยวกับคิวรี[ให้ดู รับการสนับสนุน](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

For more information or insight into your Apps in App Governance, [see Learn about visibility and insights](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview).

หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับการดูแอป โปรดดู [ดูแอป](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)ของคุณ
