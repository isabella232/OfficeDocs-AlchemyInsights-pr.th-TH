---
title: ๑๕๕๔ข้อผิดพลาด Winsock ของ Winsock ๑๐๐๖๑
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698881"
---
# <a name="winsock-error-10061"></a>ข้อผิดพลาด Winsock ๑๐๐๖๑

รหัสข้อผิดพลาดนี้หมายความว่า Microsoft ไม่สามารถสร้างซ็อกเก็ต TCP (การเชื่อมต่อ) กับโฮสต์เป้าหมายได้ สาเหตุที่น่าจะเป็นที่สุดของข้อผิดพลาดนี้เป็นปัญหาเกี่ยวกับการกำหนดค่าไฟร์วอลล์ของคุณ เมื่อต้องการแก้ไขปัญหาให้ตรวจสอบการตั้งค่าเหล่านี้:

- ตรวจสอบการกำหนดค่าไฟร์วอลล์ของคุณด้วยข้อมูลใน [Microsoft ๓๖๕ url และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- ถ้ามีข้อผิดพลาดเกิดขึ้นกับ Exchange Online Protection (EOP) คุณควรได้รับการแจ้งให้ทราบก่อนหน้านี้ไปยังการเปลี่ยนแปลงที่[อยู่ IP ของ Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- ตรวจสอบว่าผู้ให้บริการอินเทอร์เน็ตของคุณ (ISP) ไม่ได้บล็อกพอร์ต

- ตรวจสอบการตั้งค่าสมาร์ทโฮสต์และเซิร์ฟเวอร์เป้าหมายในตัวเชื่อมต่อของคุณ

โปรดสังเกตว่า Microsoft ๓๖๕ไม่ได้บล็อกการเชื่อมต่อที่ *เข้ามา* ในลักษณะนี้
