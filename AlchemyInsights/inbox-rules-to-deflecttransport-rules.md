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
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="f7956-102">กฎของโฟลว์จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน)</span><span class="sxs-lookup"><span data-stu-id="f7956-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="f7956-103">ภาพรวมทั่วไปของกฎโฟลว์จดหมาย: [กฎของโฟลว์จดหมาย (กฎการขนส่ง) ใน Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="f7956-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="f7956-104">การตั้งค่ากฎโฟลว์จดหมาย: [กระบวนงานกฎโฟลว์จดหมายใน Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="f7956-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="f7956-105">สร้างปรับเปลี่ยนและลบกฎโฟลว์จดหมาย: [จัดการกฎของลำดับจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="f7956-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="f7956-106">นอกจากนี้คุณยังสามารถจัดการกฎโฟลว์จดหมายใน Exchange Online PowerShell ได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="f7956-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="f7956-107">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (มุมมอง), [TransportRule ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (สร้าง), [เอาออก TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (ลบ), [ตั้งค่า TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (การปรับเปลี่ยนที่มีอยู่), ปิดใช้งาน [-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (ปิดใช้งานที่มีอยู่แล้ว) และ [เปิดใช้งาน-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (เปิดใช้งานที่มีอยู่แล้ว)</span><span class="sxs-lookup"><span data-stu-id="f7956-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="f7956-108">Cmdlet ของกฎโฟลว์จดหมายเพิ่มเติม: [TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดำเนินการที่พร้อมใช้งาน), [TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (รายการเงื่อนไขและข้อยกเว้นที่พร้อมใช้งาน), [ส่งออก TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (กฎการส่งออก) และ [นำเข้า-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (กฎการนำเข้า)</span><span class="sxs-lookup"><span data-stu-id="f7956-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
