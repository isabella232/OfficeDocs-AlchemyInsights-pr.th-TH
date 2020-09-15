---
title: กฎการโฟลว์จดหมายใน Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5068"
ms.openlocfilehash: 84e7b2584cd622c93e3fbb55cce41b6f9436fc24
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662992"
---
# <a name="mail-flow-transport-rules-in-exchange-online"></a><span data-ttu-id="d8958-102">กฎของโฟลว์จดหมาย (การขนส่ง) ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="d8958-102">Mail flow (transport) rules in Exchange Online</span></span>

<span data-ttu-id="d8958-103">คุณสามารถตั้งค่ากฎการขนส่งเพื่อดำเนินการกับข้อความในองค์กรของคุณปกป้องข้อความเส้นทางข้อความโดยยึดตามเกณฑ์บางอย่างเป็นต้น  เมื่อตั้งค่ากฎการขนส่งอาจใช้เวลาถึง30นาทีสำหรับกฎใหม่หรือกฎที่ได้รับการปรับปรุงที่จะนำไปใช้กับข้อความ</span><span class="sxs-lookup"><span data-stu-id="d8958-103">You can setup Transport Rules to take actions on messages in your organization, protect messages, route messages based on certain criteria, etc.  When setting up transport rules, it can take up to 30 minutes for the new or updated rule to be applied to messages.</span></span>

- <span data-ttu-id="d8958-104">ใช้ [ศูนย์การจัดการ Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) เพื่อกำหนดค่ากฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="d8958-104">Use the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) to configure Transport Rules.</span></span>

- <span data-ttu-id="d8958-105">เริ่มต้นใช้งาน[กฎโฟลว์จดหมาย (กฎการขนส่ง) ใน Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="d8958-105">Get started with how [Mail flow rules (transport rules) in Exchange Online](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rules) work.</span></span> <span data-ttu-id="d8958-106">คุณอาจต้องการทำสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="d8958-106">You may also want to:</span></span>

    - <span data-ttu-id="d8958-107">ดูขั้นตอนในการ[จัดการกฎของลำดับจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="d8958-107">View the steps to [manage mail flow rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules).</span></span>
    - <span data-ttu-id="d8958-108">วิเคราะห์[ การกระทำของกฎโฟลว์จดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions) ของคุณโดยยึดตามเงื่อนไขการจับคู่</span><span class="sxs-lookup"><span data-stu-id="d8958-108">Analyze your[ mail flow rule actions](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions) based on match conditions.</span></span>
    - <span data-ttu-id="d8958-109">[ทดสอบ](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) กฎของลำดับจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="d8958-109">[Test](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) your mail flow rules.</span></span>
