---
title: กฎของกล่องจดหมายเข้าของ๙๒๙ deflectTransport
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
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778710"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>กฎของโฟลว์จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน)

- ภาพรวมทั่วไปของกฎโฟลว์จดหมาย: [กฎของโฟลว์จดหมาย (กฎการขนส่ง) ใน Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- การตั้งค่ากฎโฟลว์จดหมาย: [กระบวนงานกฎโฟลว์จดหมายใน Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- สร้างปรับเปลี่ยนและลบกฎโฟลว์จดหมาย: [จัดการกฎของลำดับจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)

นอกจากนี้คุณยังสามารถจัดการกฎโฟลว์จดหมายใน Exchange Online PowerShell ได้อีกด้วย สำหรับข้อมูลเพิ่มเติมให้ดูที่ [TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (มุมมอง), [TransportRule ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (สร้าง), [เอาออก TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (ลบ), [ตั้งค่า TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (การปรับเปลี่ยนที่มีอยู่), ปิดใช้งาน [-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (ปิดใช้งานที่มีอยู่แล้ว) และ [เปิดใช้งาน-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (เปิดใช้งานที่มีอยู่แล้ว)

Cmdlet ของกฎโฟลว์จดหมายเพิ่มเติม: [TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดำเนินการที่พร้อมใช้งาน), [TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (รายการเงื่อนไขและข้อยกเว้นที่พร้อมใช้งาน), [ส่งออก TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (กฎการส่งออก) และ [นำเข้า-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (กฎการนำเข้า)
