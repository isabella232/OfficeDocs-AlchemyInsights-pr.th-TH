---
title: ข้อผิดพลาด 1554 Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083249"
---
# <a name="winsock-error-10061"></a>ข้อผิดพลาดของ Winsock 10061

รหัสข้อผิดพลาดนี้หมายความว่า Microsoft ไม่สามารถสร้าง SOCKET TCP (การเชื่อมต่อ) กับโฮสต์เป้าหมายได้ สาเหตุที่เป็นไปได้มากที่สุดของข้อผิดพลาดนี้คือปัญหาเกี่ยวกับการกําหนดค่าไฟร์วอลล์ของคุณ เมื่อต้องการแก้ไขปัญหา ให้ตรวจสอบการตั้งค่าเหล่านี้:

- ตรวจสอบการกําหนดค่าไฟร์วอลล์ของคุณด้วย[ข้อมูลMICROSOFT 365 URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- ถ้าข้อผิดพลาดเกิดขึ้นเฉพาะExchange Online Protection (EOP) คุณควรได้รับแจ้งก่อนหน้านี้เกี่ยวกับการเปลี่ยนแปลงExchange Online Protection [IP ของคุณ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- ตรวจสอบว่าผู้ให้บริการอินเทอร์เน็ต (ISP) ของคุณไม่ได้บล็อกพอร์ต

- ตรวจสอบการตั้งค่าสมาร์ทโฮสต์และเซิร์ฟเวอร์เป้าหมายในตัวเชื่อมต่อของคุณ

โปรดทราบว่า Microsoft 365บล็อก *การเชื่อมต่อขาเข้า* ในลักษณะนี้
