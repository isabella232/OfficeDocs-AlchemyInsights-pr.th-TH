---
title: กฎกล่องขาเข้า 929 เพื่อ deflect กฎการขนส่ง
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724611"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>กฎขั้นตอนจดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน)

- ภาพรวมทั่วไปของกฎขั้นตอนจดหมาย:[กฎการไหลของจดหมาย (กฎการขนส่ง) ในการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/jj919238.aspx)

- ตั้งค่ากฎขั้นตอนของขั้นตอนจดหมาย:[ขั้นตอนกฎขั้นตอนของกระแสจดหมายในการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/dn600436.aspx)

- สร้าง แก้ไข และลบกฎขั้นตอนจดหมาย:[จัดการกฎขั้นตอนจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)

คุณยังสามารถจัดการกฎกระแสจดหมายใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน สําหรับข้อมูลเพิ่มเติม ให้ดูที่[กฎการรับส่ง](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule)(มุมมอง),[กฎการขนส่งใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule)(สร้าง[),](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule)

cmdlet กฎกระแสจดหมายเพิ่มเติม:[รับ-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดําเนินการพร้อมใช้งาน),[รับ-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (เงื่อนไขที่มีอยู่รายการและข้อยกเว้น),[ส่งออก-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (กฎการส่งออก), และ[การนําเข้า-กฎการขนส่ง](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection)(กฎการนําเข้า)
