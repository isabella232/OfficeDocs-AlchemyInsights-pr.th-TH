---
title: "932"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766512"
---
# <a name="upgrade-azure-ad-connect"></a>ปรับรุ่นการเชื่อมต่อ AZURE AD

โดยค่าเริ่มต้น การปรับรุ่นอัตโนมัติถูกเปิดใช้งานสําหรับ Azure AD Connect ซึ่งช่วยให้คุณมั่นใจว่าคุณกําลังเรียกใช้รุ่นล่าสุด เมื่อต้องการตรวจสอบการตั้งค่าการปรับรุ่นอัตโนมัติ**Get-ADSyncAutoUpgrade** cmdlet จะส่งกลับค่าต่อไปนี้อย่างใดอย่างหนึ่ง:

- **เปิดใช้งาน**: เปิดใช้งานการปรับรุ่นอัตโนมัติ

- **ปิดใช้งาน**: การปรับรุ่นอัตโนมัติถูกปิดใช้งาน

- **ระงับ :** ระบบไม่มีสิทธิ์รับการอัพเกรดอัตโนมัติอีกต่อไป คุณไม่สามารถกําหนดค่านี้ได้ มันตั้งค่าโดยระบบ

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การอัพเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

เมื่อต้องการดาวน์โหลดการเชื่อมต่อ AD Azure รุ่นล่าสุด ให้ไปที่[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)
