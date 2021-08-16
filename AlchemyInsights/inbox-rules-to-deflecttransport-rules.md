---
title: 929 กฎกล่องจดหมายเข้าเพื่อยกเลิกการเลือกกฎทรานสพอร์ต
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
ms.openlocfilehash: a143d36d1656e205311cde4aaff3c0c21815182ee82c60039b2219addac218cb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028671"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>กฎล.ก.ล.ต. จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน)

- ภาพรวมทั่วไปของกฎล.ก.ล.ต. จดหมาย[(กฎการส่งผ่าน) Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- ตั้งค่ากฎล.ก.[ล.ต. จดหมาย ขั้นตอนกฎล](https://technet.microsoft.com/library/dn600436.aspx)Exchange Online

- สร้าง ปรับเปลี่ยน และลบกฎของล.ก.ล.จดหมาย: [จัดการกฎของลโฟลว์จดหมาย](https://technet.microsoft.com/library/jj657505.aspx)

คุณยังสามารถจัดการกฎของลExchange Onlineจดหมายใน PowerShell For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).

cmdlet กฎลนําเข้าจดหมายเพิ่มเติม: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการแอคชันที่พร้อมใช้งาน), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (รายการเงื่อนไขและข้อยกเว้นที่พร้อมใช้งาน), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (กฎการส่งออก) และ [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (กฎการนําเข้า)
