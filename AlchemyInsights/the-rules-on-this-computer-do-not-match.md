---
title: 'ข้อผิดพลาด: กฎบนคอมพิวเตอร์นี้ไม่ตรงกัน'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618032"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="806ec-102">ข้อผิดพลาด: กฎบนคอมพิวเตอร์นี้ไม่ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="806ec-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="806ec-103">เมื่อต้องการดูสถานะการปรับปรุงของปัญหาที่ทราบนี้ ให้ดูที่[กฎบนคอมพิวเตอร์นี้ไม่ตรงกับกฎบน Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="806ec-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="806ec-104">ทีม Outlook ได้ดําเนินการแก้ไขใน Build 12928.10000</span><span class="sxs-lookup"><span data-stu-id="806ec-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="806ec-105">การแก้ไขมีอยู่แล้วที่วงรับ Fast และจะไปรายเดือนช่องในปลายเดือนมิถุนายน 2020.</span><span class="sxs-lookup"><span data-stu-id="806ec-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="806ec-106">เมื่อคุณมีคงสร้างคุณอาจได้รับพร้อมท์ "กฎใดที่คุณต้องการเก็บ" หนึ่งครั้งสุดท้าย.</span><span class="sxs-lookup"><span data-stu-id="806ec-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="806ec-107">เลือกเซิร์ฟเวอร์เมื่อได้รับพร้อมท์ แล้วย้อนกลับใน Outlook และเปิดใช้งานกฎใด ๆ ที่ถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="806ec-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="806ec-108">จนกว่าการแก้ไขจะพร้อมใช้งานโปรดใช้วิธีแก้ปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="806ec-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="806ec-109">**วิธีแก้ปัญหา**: ในรายงานล่าสุด</span><span class="sxs-lookup"><span data-stu-id="806ec-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="806ec-110">ถ้าคุณยังทํางานเป็นปัญหา ให้พิจารณาการลบกฎ แล้วสร้าง และแก้ไขกฎใน OWA (Outlook Web App) จนกว่าปัญหาได้รับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="806ec-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="806ec-111">ถ้าคุณไม่สามารถลบกฎด้วยตนเองคุณสามารถเรียกใช้คําสั่ง Outlook เมื่อคุณเริ่ม Outlook โดยการเรียกใช้ Outlook.exe /cleanrules</span><span class="sxs-lookup"><span data-stu-id="806ec-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="806ec-112">นี้จะลบทั้งไคลเอ็นต์และกฎของเซิร์ฟเวอร์</span><span class="sxs-lookup"><span data-stu-id="806ec-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="806ec-113">มันจะลบกฎทั้งหมดสําหรับบัญชีทั้งหมดในโปรไฟล์ Outlook</span><span class="sxs-lookup"><span data-stu-id="806ec-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="806ec-114">คําสั่งนี้ได้รับการบันทึกเพิ่มเติมในบทความสวิตช์บรรทัดคําสั่ง</span><span class="sxs-lookup"><span data-stu-id="806ec-114">This command is further documented in the Command-line switches  article.</span></span>