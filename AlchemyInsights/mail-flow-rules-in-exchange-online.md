---
title: กฎลโฟลว์ของจดหมายใน Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5068"
ms.openlocfilehash: 737e0f2db14a766db1c21720a936c2dd4645aef3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810575"
---
# <a name="mail-flow-transport-rules-in-exchange-online"></a><span data-ttu-id="6daef-102">กฎของลโฟลว์จดหมาย (การส่งผ่าน) ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6daef-102">Mail flow (transport) rules in Exchange Online</span></span>

<span data-ttu-id="6daef-103">คุณสามารถตั้งค่ากฎการส่งผ่านเพื่อจัดการข้อความในองค์กรของคุณ ป้องกันข้อความ เส้นทางข้อความตามเกณฑ์บางอย่าง และอื่นๆ  เมื่อตั้งค่ากฎการส่งผ่าน อาจใช้เวลาถึง 30 นาทีเพื่อปรับใช้กฎใหม่หรือกฎที่อัปเดตกับข้อความ</span><span class="sxs-lookup"><span data-stu-id="6daef-103">You can setup Transport Rules to take actions on messages in your organization, protect messages, route messages based on certain criteria, etc.  When setting up transport rules, it can take up to 30 minutes for the new or updated rule to be applied to messages.</span></span>

- <span data-ttu-id="6daef-104">ใช้ศูนย์ [การจัดการ Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) เพื่อกําหนดค่ากฎการส่งผ่าน</span><span class="sxs-lookup"><span data-stu-id="6daef-104">Use the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) to configure Transport Rules.</span></span>

- <span data-ttu-id="6daef-105">เริ่มต้นใช้งานเกี่ยวกับวิธีที่กฎ[ของลโฟลว์ของจดหมาย (กฎการส่งผ่าน) ในการงานของ Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="6daef-105">Get started with how [Mail flow rules (transport rules) in Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules) work.</span></span> <span data-ttu-id="6daef-106">คุณอาจต้องการ:</span><span class="sxs-lookup"><span data-stu-id="6daef-106">You may also want to:</span></span>

    - <span data-ttu-id="6daef-107">ดูขั้นตอนในการจัดการ [กฎของล.ก](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules). จดหมาย</span><span class="sxs-lookup"><span data-stu-id="6daef-107">View the steps to [manage mail flow rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules).</span></span>
    - <span data-ttu-id="6daef-108">วิเคราะห์การ[ แอคชันของกฎการโฟลว์](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions) จดหมายของคุณโดยยึดตามเงื่อนไขการจับคู่</span><span class="sxs-lookup"><span data-stu-id="6daef-108">Analyze your[ mail flow rule actions](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions) based on match conditions.</span></span>
    - <span data-ttu-id="6daef-109">[ทดสอบ](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) กฎการโฟลว์จดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="6daef-109">[Test](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) your mail flow rules.</span></span>
