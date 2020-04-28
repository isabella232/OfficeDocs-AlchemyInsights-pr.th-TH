---
title: กฎของขั้นตอนจดหมายในการแลกเปลี่ยนแบบออนไลน์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5068"
ms.openlocfilehash: 09adcce1f7124771d6c0a1aaca44337dc02d18c2
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915268"
---
# <a name="mail-flow-transport-rules-in-exchange-online"></a><span data-ttu-id="339be-102">กฎกระแสจดหมาย (การขนส่ง) ใน Exchange แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="339be-102">Mail flow (transport) rules in Exchange Online</span></span>

<span data-ttu-id="339be-103">คุณสามารถตั้งค่ากฎการส่งผ่านเพื่อดําเนินการกับข้อความในองค์กรของคุณ, ป้องกันข้อความ, กําหนดเส้นทางข้อความตามเกณฑ์บางอย่าง, ฯลฯ.  เมื่อตั้งค่ากฎการขนส่ง อาจใช้เวลาถึง 30 นาทีสําหรับกฎใหม่หรือกฎที่ปรับปรุงแล้วที่จะใช้กับข้อความ</span><span class="sxs-lookup"><span data-stu-id="339be-103">You can setup Transport Rules to take actions on messages in your organization, protect messages, route messages based on certain criteria, etc.  When setting up transport rules, it can take up to 30 minutes for the new or updated rule to be applied to messages.</span></span>

- <span data-ttu-id="339be-104">ใช้[ศูนย์ดูแล Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) เพื่อกําหนดค่ากฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="339be-104">Use the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) to configure Transport Rules.</span></span>

- <span data-ttu-id="339be-105">เริ่มต้นใช้งานอย่างไร[กฎขั้นตอนจดหมาย (กฎการขนส่ง) ใน Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="339be-105">Get started with how [Mail flow rules (transport rules) in Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules) work.</span></span> <span data-ttu-id="339be-106">คุณอาจต้องการ:</span><span class="sxs-lookup"><span data-stu-id="339be-106">You may also want to:</span></span>

    - <span data-ttu-id="339be-107">ดูขั้นตอนในการจัดการ[กฎขั้นตอนจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="339be-107">View the steps to [manage mail flow rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules).</span></span>
    - <span data-ttu-id="339be-108">วิเคราะห์[การดําเนินการกฎโฟลว์จดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions)ของคุณตามเงื่อนไขการจับคู่</span><span class="sxs-lookup"><span data-stu-id="339be-108">Analyze your[ mail flow rule actions](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions) based on match conditions.</span></span>
    - <span data-ttu-id="339be-109">[ทดสอบ](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)กฎขั้นตอนจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="339be-109">[Test](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) your mail flow rules.</span></span>
