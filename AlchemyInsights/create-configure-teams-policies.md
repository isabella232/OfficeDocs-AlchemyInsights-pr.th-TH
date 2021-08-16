---
title: สร้างและกําหนดค่าTeamsนโยบาย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12851"
- "9000734"
ms.openlocfilehash: 6e4a61c7d723486c98737edacebb671e44cb75a618872a37098642021aa70c38
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874450"
---
# <a name="create-and-configure-teams-policies"></a>สร้างและกําหนดค่าTeamsนโยบาย

คุณสามารถสร้างนโยบายที่ช่วยจัดการประสบการณ์Teamsการใช้งานจริงขององค์กรของคุณ เมื่อต้องการกําหนดค่านโยบาย คุณสามารถแก้ไขนโยบายส่วนกลางหรือสร้างนโยบายในศูนย์Teams[ผู้ดูแลระบบ](https://admin.microsoft.com/)[และกําหนดนโยบายให้กับ](https://docs.microsoft.com/microsoftteams/assign-policies)ผู้ใช้ Global policies are set as default for all users and automatically assigned when you create a user in Teams.

**หมายเหตุ:** การเปลี่ยนแปลงนโยบายใช้เวลาอย่างน้อย 4 ชั่วโมงและสูงสุด 48 ชั่วโมงเพื่อให้มีผล 

ดูข้อมูลเพิ่มเติมที่[จัดการTeamsด้วย](https://docs.microsoft.com/microsoftteams/manage-teams-with-policies)นโยบาย

ต่อไปนี้เป็นการตั้งค่าทั่วไปสองสามรายการที่ได้รับการสนับสนุนโดยนโยบาย:

- Teamsสนับสนุน[นโยบายการเก็บ](https://docs.microsoft.com/microsoftteams/retention-policies)ข้อมูลแชทและข้อความในแชนเนลเพื่อให้ผู้ดูแลระบบสามารถตัดสินใจว่าจะเก็บข้อมูล ลบ หรือเก็บรักษาไว้ในช่วงเวลาหนึ่งแล้วจึงลบออก For more information about policies in the ศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365, see [Learn about retention for Teams](https://docs.microsoft.com/microsoftteams/assign-policies).
- Teamsนโยบายสมุดรายชื่อจะถูกตั้งค่าผ่านการค้นหาไดเรกทอรีที่จัดขอบเขตไว้ For more information, see [use Microsoft Teams scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).
- นโยบายการประชุมจะควบคุมสิ่งที่ผู้ใช้สามารถTeamsการประชุมรวมถึงการควบคุมล็อบบี้ การแชทในการประชุม การบันทึกการประชุม และอื่นๆ For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
- นโยบายการส่งข้อความจะควบคุมการแชทและข้อความ รวมถึงการบล็อกการแชทและใบตอบรับการอ่าน ดูข้อมูลเพิ่มเติมที่[จัดการนโยบายการส่งข้อความใน Teams](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)
- นโยบายการตั้งค่าแอปจะควบคุมการติดตั้ง การอัปโหลด และการปักหมุดแอป ดูข้อมูลเพิ่มเติมที่[จัดการนโยบายการตั้งค่าแอปใน Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies)
- ใช้นโยบายการโทรเพื่อกําหนดค่าการโทรส่วนบุคคลและการโอนสายเรียกเข้า For more information, see [Calling and call-forwarding in Teams](https://docs.microsoft.com/MicrosoftTeams/teams-calling-policy).

