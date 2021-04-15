---
title: 'ข้อผิดพลาด: กฎบนคอมพิวเตอร์นี้ไม่ตรงกัน'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782971"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="e0c41-102">ข้อผิดพลาด: กฎบนคอมพิวเตอร์นี้ไม่ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="e0c41-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="e0c41-103">เมื่อต้องการดูสถานะที่อัปเดตของปัญหาที่ทราบนี้ ให้ดู [กฎบนคอมพิวเตอร์นี้ไม่ตรงกับกฎบน Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="e0c41-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="e0c41-104">ทีม Outlook ได้ดําเนินการแก้ไขในรุ่น 12928.10000</span><span class="sxs-lookup"><span data-stu-id="e0c41-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="e0c41-105">การแก้ไขมีอยู่แล้วใน Insider ที่เร็วก่อนแล้วและจะไปอยู่ในแชนเนลรายเดือนในช่วงปลายเดือนมิถุนายน 2020</span><span class="sxs-lookup"><span data-stu-id="e0c41-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="e0c41-106">เมื่อคุณมีบิลด์ที่แก้ไขแล้ว คุณอาจได้รับพร้อมท์ "คุณต้องการเก็บกฎใด" เป็นครั้งสุดท้าย</span><span class="sxs-lookup"><span data-stu-id="e0c41-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="e0c41-107">เลือกเซิร์ฟเวอร์เมื่อได้รับพร้อมท์ แล้วย้อนกลับไปใน Outlook และเปิดใช้งานกฎใดๆ ที่ถูกปิดใช้งานอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e0c41-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="e0c41-108">จนกว่าการแก้ไขจะพร้อมใช้งาน โปรดใช้วิธีแก้ไขปัญหาชั่วคราวต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e0c41-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="e0c41-109">**วิธี** แก้ไขปัญหาชั่วคราว : ในรายงานล่าสุด ปัญหานี้เกิดขึ้นกับผู้ที่สร้างกฎของไคลเอ็นต์ใน Outlook บนเดสก์ท็อปเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="e0c41-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="e0c41-110">ถ้าคุณยังคงประสบปัญหา ให้พิจารณาลบกฎ แล้วสร้างและแก้ไขกฎเฉพาะใน OWA (Outlook Web App) จนกว่าปัญหาจะได้รับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="e0c41-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="e0c41-111">ถ้าคุณไม่สามารถลบกฎด้วยตนเอง คุณสามารถเรียกใช้สั่ง Outlook เมื่อคุณเริ่ม Outlook โดยการเรียกใช้ Outlook.exe /cleanrules</span><span class="sxs-lookup"><span data-stu-id="e0c41-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="e0c41-112">การนี่จะลบทั้งกฎของไคลเอ็นต์และเซิร์ฟเวอร์</span><span class="sxs-lookup"><span data-stu-id="e0c41-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="e0c41-113">ซึ่งจะลบกฎทั้งหมดออกจากบัญชีทั้งหมดในโปรไฟล์ Outlook</span><span class="sxs-lookup"><span data-stu-id="e0c41-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="e0c41-114">มีเอกสารเพิ่มเติมอยู่ในบทความ สวิตช์บรรทัดการสั่ง</span><span class="sxs-lookup"><span data-stu-id="e0c41-114">This command is further documented in the Command-line switches article.</span></span>

