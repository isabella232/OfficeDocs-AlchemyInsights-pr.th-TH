---
title: 932 การอัปเกรด AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104831"
---
# <a name="upgrade-azure-ad-connect"></a>อัปเกรด Azure AD เชื่อมต่อ

ตามค่าเริ่มต้น การอัปเกรดอัตโนมัติจะเปิดใช้งานเชื่อมต่อ Azure AD ซึ่งจะช่วยตรวจสอบให้แน่ใจว่าคุณใช้เวอร์ชันล่าสุด เมื่อต้องการตรวจสอบการตั้งค่าการอัปเกรดอัตโนมัติ ให้ใช้ **cmdlet Get-ADSyncAutoUpgrady** ใน Azure AD PowerShell cmdlet จะส่งกลับค่าใดค่าหนึ่งต่อไปนี้

- **เปิดใช้งาน**: เปิดใช้งานการอัปเกรดอัตโนมัติ

- **ปิดใช้งาน**: การอัปเกรดอัตโนมัติถูกปิดใช้งาน

- **ถูกระงับ**: ระบบไม่มีสิทธิ์ในการรับการอัปเกรดอัตโนมัติอีกต่อไป คุณไม่สามารถกําหนดค่านี้ ถูกตั้งค่าโดยระบบ

ดูข้อมูลเพิ่มเติมเกี่ยวกับ [การอัปเกรด](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)โดยอัตโนมัติ

เมื่อต้องการดาวน์โหลดเวอร์ชันล่าสุดของ Azure AD เชื่อมต่อ ให้ [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) ไปยัง
