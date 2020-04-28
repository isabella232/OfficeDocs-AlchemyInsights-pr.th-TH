---
title: การใช้ DLP ในกฎการขนส่ง
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
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915297"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="9e832-102">การใช้ DLP ในกฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="9e832-102">Using DLP in transport rules</span></span>

<span data-ttu-id="9e832-103">เมื่อต้องการรวมการป้องกันข้อมูลสูญหาย (DLP) ลงในการขนส่งที่มีอยู่ ให้ใช้เงื่อนไข "**ถ้าข้อความมี... ข้อมูลที่สําคัญ**" ในการตั้งค่ากฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="9e832-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="9e832-104">**สําหรับรายละเอียดเพิ่มเติม โปรดดูที่:**</span><span class="sxs-lookup"><span data-stu-id="9e832-104">**For more details, see:**</span></span>

- <span data-ttu-id="9e832-105">ชนิดข้อมูลที่ละเอียดอ่อน DLP แบบรวมในกฎการขนส่ง:[รวมกฎข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)</span><span class="sxs-lookup"><span data-stu-id="9e832-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="9e832-106">นอกจากนี้คุณยังสามารถทดสอบกฎที่มีหรือไม่มีการทดสอบนโยบายโดยใช้โหมดทดสอบในกฎ</span><span class="sxs-lookup"><span data-stu-id="9e832-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="9e832-107">คุณควรรอ 30 นาทีหลังจากสร้างกฎก่อนที่จะทดสอบมัน.</span><span class="sxs-lookup"><span data-stu-id="9e832-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="9e832-108">ดู[ทดสอบกฎลําดับ/การขนส่งจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="9e832-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="9e832-109">**หมายเหตุ**: ถ้าคุณกําลังพยายามใช้นโยบาย DLP ใหม่ กับกฎการขนส่งใน EAC ใช้[นโยบาย DLP ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)แทน</span><span class="sxs-lookup"><span data-stu-id="9e832-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
