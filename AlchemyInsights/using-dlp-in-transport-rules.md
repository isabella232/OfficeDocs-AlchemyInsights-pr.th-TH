---
title: การใช้ DLP ในกฎการส่งผ่าน
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
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827235"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="c2400-102">การใช้ DLP ในกฎการส่งผ่าน</span><span class="sxs-lookup"><span data-stu-id="c2400-102">Using DLP in transport rules</span></span>

<span data-ttu-id="c2400-103">เมื่อต้องการรวมการป้องกันการสูญหายของข้อมูล (DLP) ลงในการส่งผ่านที่มีอยู่ ให้ใช้เงื่อนไข "**ถ้าข้อความมี... ข้อมูลที่ละเอียดอ่อน**" ในการตั้งค่ากฎการส่งผ่าน</span><span class="sxs-lookup"><span data-stu-id="c2400-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="c2400-104">**ดูรายละเอียดเพิ่มเติมที่:**</span><span class="sxs-lookup"><span data-stu-id="c2400-104">**For more details, see:**</span></span>

- <span data-ttu-id="c2400-105">ชนิดข้อมูลที่เป็นความลับ DLP ที่รวมในกฎการส่งผ่าน:[รวมกฎของข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)</span><span class="sxs-lookup"><span data-stu-id="c2400-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="c2400-106">คุณยังสามารถทดสอบกฎที่มีหรือไม่ทดสอบนโยบายโดยใช้ โหมดการทดสอบ บนกฎได้</span><span class="sxs-lookup"><span data-stu-id="c2400-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="c2400-107">คุณควรรอ 30 นาทีหลังจากสร้างกฎก่อนการทดสอบ</span><span class="sxs-lookup"><span data-stu-id="c2400-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="c2400-108">ดู [ทดสอบกฎของลโฟลว์/การส่งผ่านจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="c2400-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="c2400-109">**หมายเหตุ**: ถ้าคุณพยายามปรับใช้นโยบาย DLP ใหม่กับกฎการส่งผ่านใน EAC ให้ใช้ [นโยบาย DLP ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) แทน</span><span class="sxs-lookup"><span data-stu-id="c2400-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
