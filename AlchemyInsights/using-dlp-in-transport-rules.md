---
title: การใช้ DLP ในกฎการขนส่ง
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
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773182"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="68d6c-102">การใช้ DLP ในกฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="68d6c-102">Using DLP in transport rules</span></span>

<span data-ttu-id="68d6c-103">เมื่อต้องการรวมการป้องกันการสูญหายของข้อมูล (DLP) ลงในการขนส่งที่มีอยู่ให้ใช้เงื่อนไข "**ถ้าข้อความมี ... ข้อมูลที่ละเอียดอ่อน**"ในการตั้งค่ากฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="68d6c-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="68d6c-104">**สำหรับรายละเอียดเพิ่มเติมให้ดูที่:**</span><span class="sxs-lookup"><span data-stu-id="68d6c-104">**For more details, see:**</span></span>

- <span data-ttu-id="68d6c-105">ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ที่รวมอยู่ในกฎการขนส่ง:[รวมกฎข้อมูลที่สำคัญ](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)</span><span class="sxs-lookup"><span data-stu-id="68d6c-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="68d6c-106">นอกจากนี้คุณยังสามารถทดสอบกฎที่มีหรือไม่มีการทดสอบนโยบายโดยใช้โหมดทดสอบบนกฎได้</span><span class="sxs-lookup"><span data-stu-id="68d6c-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="68d6c-107">คุณควรรอ30นาทีหลังจากสร้างกฎก่อนที่จะทดสอบ</span><span class="sxs-lookup"><span data-stu-id="68d6c-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="68d6c-108">ดู [ทดสอบการรับส่งจดหมาย/กฎการขนส่ง](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="68d6c-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="68d6c-109">**หมายเหตุ**: ถ้าคุณกำลังพยายามดำเนินการนโยบาย DLP ใหม่กับกฎการส่งผ่านใน EAC ให้ใช้ [นโยบาย dlp ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) แทน</span><span class="sxs-lookup"><span data-stu-id="68d6c-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
