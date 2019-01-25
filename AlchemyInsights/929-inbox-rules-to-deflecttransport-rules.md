---
title: กฎของกล่องขาเข้า 929 deflectTransport กฎ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: ed4afe938b310f1569061ad00bf90ad87e91b465
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493213"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>กฎสำหรับลำดับจดหมาย (หรือที่เรียกอีกอย่างหนึ่งว่ากฎขนส่ง)

- ภาพรวมทั่วไปของกฎกระแสจดหมาย:[จดหมายไหลกฎ (กฎการขนส่ง) ใน Exchange แบบออนไลน์](https://technet.microsoft.com/library/jj919238.aspx)
    
- ตั้งค่ากฎลำดับจดหมาย:[จดหมายไหลขั้นตอนกฎการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/dn600436.aspx)
    
- สร้าง แก้ไข และลบกฎกระแสจดหมาย:[จัดการกฎสำหรับลำดับจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)
    
นอกจากนี้คุณสามารถจัดการกฎกระแสจดหมายใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน สำหรับข้อมูลเพิ่มเติม ให้ดูที่[TransportRule รับ](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule)(มุมมอง), [TransportRule ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule)(create),[เอา TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (ลบ)[ชุด TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (ปรับเปลี่ยนที่มีอยู่),[ปิดการใช้งาน TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (ปิดการใช้งานที่มีอยู่), และ [เปิดใช้งาน TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (เปิดใช้งานอยู่) 
  
Cmdlet ของกฎของกระแสจดหมายเพิ่มเติม:[รับ TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดำเนินการพร้อมใช้งาน),[เรียก TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (เงื่อนไขที่พร้อมใช้งานรายการและข้อยกเว้น),[ส่งออก TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (ส่งออกกฎ), และ[ นำเข้า-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (นำเข้ากฎกฎ) 
  

