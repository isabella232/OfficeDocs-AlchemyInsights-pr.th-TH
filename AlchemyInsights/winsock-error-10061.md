---
title: ข้อผิดพลาด 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766188"
---
# <a name="winsock-error-10061"></a>ข้อผิดพลาด 10061 ของวินซอค

รหัสข้อผิดพลาดนี้หมายความ ว่า Microsoft ไม่สามารถสร้างซ็อกเก็ต TCP (การเชื่อมต่อ) กับโฮสต์เป้าหมาย สาเหตุส่วนใหญ่ของข้อผิดพลาดนี้คือปัญหากับการกําหนดค่าไฟร์วอลล์ของคุณ เมื่อต้องการแก้ไขปัญหา ให้ตรวจสอบการตั้งค่าเหล่านี้:

- ตรวจสอบการกําหนดค่าไฟร์วอลล์ของคุณด้วยข้อมูลใน[Url ของ Microsoft 365 และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- ถ้าข้อผิดพลาดเป็นเฉพาะกับการป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน (EOP), คุณควรได้รับแจ้งก่อนหน้านี้การเปลี่ยนแปลงไปยัง[ที่อยู่ IP ป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- ตรวจสอบว่าผู้ให้บริการอินเทอร์เน็ต (ISP) ของคุณไม่ได้บล็อกพอร์ต

- ตรวจสอบการตั้งค่าโฮสต์สมาร์ทและเซิร์ฟเวอร์เป้าหมายในตัวเชื่อมต่อของคุณ

โปรดสังเกตว่า Microsoft 365 ไม่บล็อกการเชื่อมต่อ*ขาเข้า*ในลักษณะนี้
