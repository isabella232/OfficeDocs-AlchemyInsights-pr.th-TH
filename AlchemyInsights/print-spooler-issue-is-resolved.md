---
title: ปัญหาตัวจัดคิวงานพิมพ์ได้รับการแก้ไขแล้ว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088527"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="5c95c-102">ปัญหาตัวจัดคิวงานพิมพ์ได้รับการแก้ไขแล้ว</span><span class="sxs-lookup"><span data-stu-id="5c95c-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="5c95c-103">หากอุปกรณ์ของคุณได้รับการอัปเดตด้วย Windows 10 **OS Build 19041.329**คุณอาจสังเกตเห็นปัญหาที่ทําให้เครื่องพิมพ์บางเครื่องไม่สามารถพิมพ์ได้</span><span class="sxs-lookup"><span data-stu-id="5c95c-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="5c95c-104">ตัวจัดคิวงานพิมพ์อาจแสดงข้อผิดพลาด หรือปิดโดยไม่คาดคิดเมื่อพยายามพิมพ์ และไม่มีผลลัพธ์ใดมาจากเครื่องพิมพ์ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="5c95c-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="5c95c-105">ปัญหานี้แก้ไขได้ในระบบปฏิบัติการรุ่น**19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)</span><span class="sxs-lookup"><span data-stu-id="5c95c-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="5c95c-106">**การสืบสวนอย่างต่อเนื่อง**</span><span class="sxs-lookup"><span data-stu-id="5c95c-106">**Ongoing investigation**</span></span>

<span data-ttu-id="5c95c-107">แฟ้มบริการระบบย่อย (LSASS)\*\* (Isass.exe)\*\* อาจล้มเหลวบนอุปกรณ์บางอย่างที่มีข้อความแสดงข้อผิดพลาด "กระบวนการระบบที่สําคัญ C:\WINDOWS\system32\Isass.exe ล้มเหลวด้วยรหัสสถานะ c0000008</span><span class="sxs-lookup"><span data-stu-id="5c95c-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="5c95c-108">เครื่องต้องเริ่มต้นใหม่"</span><span class="sxs-lookup"><span data-stu-id="5c95c-108">The machine must now be restarted".</span></span>  <span data-ttu-id="5c95c-109">**Microsoft กําลังทํางานเกี่ยวกับความละเอียด และจะมีการปรับปรุงในรุ่นต่อไป**</span><span class="sxs-lookup"><span data-stu-id="5c95c-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="5c95c-110">สําหรับข้อมูลเพิ่มเติม โปรดตรวจสอบ[ปัญหา Windows 10 เวอร์ชัน 2004 ที่ทราบ](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)</span><span class="sxs-lookup"><span data-stu-id="5c95c-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>