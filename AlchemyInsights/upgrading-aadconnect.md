---
title: ๙๓๒การอัปเกรด AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806058"
---
# <a name="upgrade-azure-ad-connect"></a>การอัปเกรด Azure AD Connect

ตามค่าเริ่มต้นการอัปเกรดอัตโนมัติจะถูกเปิดใช้งานสำหรับ Azure AD Connect ซึ่งจะช่วยให้แน่ใจว่าคุณกำลังใช้งานเวอร์ชันล่าสุด เมื่อต้องการตรวจสอบการตั้งค่าการอัปเกรดอัตโนมัติให้ใช้ cmdlet **รับ ADSyncAutoUpgrade** ใน PowerShell AD Azure Cmdlet นี้จะส่งกลับค่าใดค่าหนึ่งดังต่อไปนี้

- **เปิดใช้**งาน: เปิดใช้งานการอัปเกรดอัตโนมัติ

- **ปิดใช้**งาน: การอัปเกรดอัตโนมัติถูกปิดใช้งาน

- **ถูกระงับ**: ระบบจะไม่มีสิทธิ์ในการรับการอัปเกรดอัตโนมัติอีกต่อไป คุณไม่สามารถกำหนดค่านี้ได้ ระบบจะตั้งค่าโดยระบบ

สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[อัปเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

เมื่อต้องการดาวน์โหลดเวอร์ชันล่าสุดของ Azure AD [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) Connect ให้ไปที่
