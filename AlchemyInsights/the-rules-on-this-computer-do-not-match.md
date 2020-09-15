---
title: 'ข้อผิดพลาด: กฎบนคอมพิวเตอร์เครื่องนี้ไม่ตรงกัน'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690982"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="69b14-102">ข้อผิดพลาด: กฎบนคอมพิวเตอร์เครื่องนี้ไม่ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="69b14-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="69b14-103">เมื่อต้องการดูสถานะการอัปเดตของปัญหาที่ทราบแล้วนี้ให้ดู [ที่กฎบนคอมพิวเตอร์เครื่องนี้ไม่ตรงกับกฎบน Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="69b14-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="69b14-104">ทีม Outlook ได้ดำเนินการแก้ไขในรุ่น๑๒๙๒๘.๑๐๐๐๐</span><span class="sxs-lookup"><span data-stu-id="69b14-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="69b14-105">การแก้ไขมีอยู่แล้วใน Insider ที่รวดเร็วและจะไปที่แชนเนลรายเดือนในช่วงปลายเดือนมิถุนายน๒๐๒๐</span><span class="sxs-lookup"><span data-stu-id="69b14-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="69b14-106">เมื่อคุณมีการสร้างแบบคงที่คุณอาจได้รับพร้อมท์ "กฎใดที่คุณต้องการเก็บ" หนึ่งครั้งสุดท้าย</span><span class="sxs-lookup"><span data-stu-id="69b14-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="69b14-107">เลือกเซิร์ฟเวอร์เมื่อได้รับพร้อมท์จากนั้นกลับไปที่ Outlook แล้วเปิดใช้งานกฎใดๆที่ถูกปิดใช้งานอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="69b14-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="69b14-108">จนกว่าจะมีการแก้ไขปัญหาโปรดใช้วิธีแก้ไขปัญหาชั่วคราวต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="69b14-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="69b14-109">**วิธีแก้ไขปัญหาชั่ว**คราว: ในรายงานล่าสุดปัญหานี้เกิดขึ้นสำหรับผู้ที่ได้สร้างเฉพาะกฎของไคลเอ็นต์ใน Outlook บนเดสก์ท็อปเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="69b14-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="69b14-110">ถ้าคุณยังคงพบปัญหาอยู่ให้ลองลบกฎแล้วสร้างและแก้ไขกฎเฉพาะใน OWA (Outlook Web App) จนกว่าปัญหาจะได้รับการแก้ไขแล้ว</span><span class="sxs-lookup"><span data-stu-id="69b14-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="69b14-111">ถ้าคุณไม่สามารถลบกฎด้วยตนเองคุณสามารถเรียกใช้คำสั่ง Outlook เมื่อคุณเริ่มใช้งาน Outlook โดยการเรียกใช้ Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="69b14-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="69b14-112">การทำเช่นนี้จะลบทั้งกฎของไคลเอ็นต์และเซิร์ฟเวอร์</span><span class="sxs-lookup"><span data-stu-id="69b14-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="69b14-113">ซึ่งจะเป็นการลบกฎทั้งหมดของบัญชีผู้ใช้ทั้งหมดในโปรไฟล์ Outlook</span><span class="sxs-lookup"><span data-stu-id="69b14-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="69b14-114">คำสั่งนี้จะได้รับการบันทึกเพิ่มเติมในบทความสวิตช์บรรทัดคำสั่ง</span><span class="sxs-lookup"><span data-stu-id="69b14-114">This command is further documented in the Command-line switches article.</span></span>

