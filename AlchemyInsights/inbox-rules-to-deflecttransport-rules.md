---
title: กฎของกล่องขาเข้า 929 deflectTransport กฎ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 140cb6e85d0f08393439b023578457998a84dc62
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499622"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="b502f-102">กฎสำหรับลำดับจดหมาย (หรือที่เรียกอีกอย่างหนึ่งว่ากฎขนส่ง)</span><span class="sxs-lookup"><span data-stu-id="b502f-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="b502f-103">ภาพรวมทั่วไปของกฎกระแสจดหมาย:[จดหมายไหลกฎ (กฎการขนส่ง) ใน Exchange แบบออนไลน์](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="b502f-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="b502f-104">ตั้งค่ากฎลำดับจดหมาย:[จดหมายไหลขั้นตอนกฎการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="b502f-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="b502f-105">สร้าง แก้ไข และลบกฎกระแสจดหมาย:[จัดการกฎสำหรับลำดับจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="b502f-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="b502f-106">นอกจากนี้คุณสามารถจัดการกฎกระแสจดหมายใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="b502f-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="b502f-107">สำหรับข้อมูลเพิ่มเติม ให้ดูที่[TransportRule รับ](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule)(มุมมอง), [TransportRule ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule)(create),[เอา TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (ลบ)[ชุด TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (ปรับเปลี่ยนที่มีอยู่),[ปิดการใช้งาน TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (ปิดการใช้งานที่มีอยู่), และ [เปิดใช้งาน TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (เปิดใช้งานอยู่)</span><span class="sxs-lookup"><span data-stu-id="b502f-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="b502f-108">Cmdlet ของกฎของกระแสจดหมายเพิ่มเติม:[รับ TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดำเนินการพร้อมใช้งาน),[เรียก TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (เงื่อนไขที่พร้อมใช้งานรายการและข้อยกเว้น),[ส่งออก TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (ส่งออกกฎ), และ[ นำเข้า-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (นำเข้ากฎกฎ)</span><span class="sxs-lookup"><span data-stu-id="b502f-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
