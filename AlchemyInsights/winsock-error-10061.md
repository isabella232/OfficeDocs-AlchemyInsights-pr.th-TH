---
title: ข้อผิดพลาด Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757129"
---
# <a name="winsock-error-10061"></a>ข้อผิดพลาด Winsock 10061

รหัสข้อผิดพลาดนี้หมายความ ว่า Office 365 ไม่สามารถสร้างซ็อกเก็ต TCP (เชื่อมต่อ) กับโฮสต์เป้าหมาย สาเหตุของข้อผิดพลาดนี้น่ามีปัญหากับการกำหนดค่าไฟร์วอลล์ของคุณ เมื่อต้องการแก้ไขปัญหา ตรวจสอบการตั้งค่าเหล่านี้:

- ตรวจสอบการกำหนดค่าไฟร์วอลล์ของคุณกับข้อมูลใน[Office 365 Url และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- ถ้าข้อผิดพลาดมีการระบุการแลกเปลี่ยนแบบออนไลน์ป้องกัน (EOP), คุณควรได้รับก่อนหน้านี้แจ้งการเปลี่ยนแปลง[ที่อยู่ IP ป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- ตรวจสอบว่า ผู้ให้บริการอินเทอร์เน็ต (ISP) ของคุณไม่ได้บล็อกพอร์ต

- ตรวจสอบแบบสมาร์ทโฮสต์และเป้าหมายการตั้งค่าเซิร์ฟเวอร์ในตัวเชื่อมต่อของคุณ

หมายเหตุว่า Office 365 ไม่บล็อกการเชื่อมต่อ*ขาเข้า*ในลักษณะนี้
