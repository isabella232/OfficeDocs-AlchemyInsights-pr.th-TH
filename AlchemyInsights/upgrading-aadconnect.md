---
title: AADConnect การปรับรุ่น 932
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389782"
---
# <a name="upgrade-azure-ad-connect"></a>การเชื่อมต่อ Azure AD การปรับรุ่น

โดยค่าเริ่มต้น การอัพเกรดอัตโนมัติถูกเปิดใช้งานสำหรับการเชื่อมต่อ AD Azure ซึ่งช่วยให้แน่ใจว่าคุณกำลังเรียกใช้รุ่นล่าสุด เมื่อต้องการตรวจสอบการตั้งค่าการปรับรุ่นอัตโนมัติ ใช้ cmdlet การ**ADSyncAutoUpgrade รับ**ใน PowerShell โฆษณา Azure Cmdlet นี้จะส่งกลับค่าหนึ่งค่าต่อไปนี้: 

- **เปิดการใช้งาน**: เปิดใช้งานการปรับรุ่นโดยอัตโนมัติ

- **ปิดการใช้งาน**: การอัพเกรดอัตโนมัติถูกปิดใช้งาน

- **ระงับ**: ระบบไม่มีสิทธิ์ได้รับการปรับรุ่นโดยอัตโนมัติ คุณไม่สามารถกำหนดค่านี้ จะถูกกำหนด โดยระบบ 

สำหรับข้อมูลเพิ่มเติม ดู[การอัพเกรดโดยอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

เมื่อต้องการดาวน์โหลดรุ่นล่าสุดของการเชื่อมต่อ AD Azure ไป[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)
