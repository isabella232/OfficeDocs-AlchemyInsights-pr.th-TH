---
title: เรียกใช้การวินิจฉัยหน่วยความจํา Windows ใน Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826686"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="192d8-102">เรียกใช้การวินิจฉัยหน่วยความจํา Windows ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="192d8-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="192d8-103">หาก Windows และแอปบนพีซีของคุณหยุดการหยุดหรือเกิดการผิดพลาด คุณอาจมีปัญหากับหน่วยความจําพีซี (RAM)</span><span class="sxs-lookup"><span data-stu-id="192d8-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="192d8-104">คุณสามารถเรียกใช้การวินิจฉัยหน่วยความจําของ Windows เพื่อตรวจสอบปัญหาเกี่ยวกับ RAM ของพีซี</span><span class="sxs-lookup"><span data-stu-id="192d8-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="192d8-105">ในกล่องค้นหาบนแถบงานของคุณ พิมพ์ การวินิจฉัย **หน่วยความ** จํา แล้วเลือก **การวินิจฉัยหน่วยความจํา Windows**</span><span class="sxs-lookup"><span data-stu-id="192d8-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="192d8-106">เมื่อต้องการเรียกใช้การวินิจฉัย พีซีต้องรีสตาร์ต</span><span class="sxs-lookup"><span data-stu-id="192d8-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="192d8-107">คุณมีตัวเลือกในการรีสตาร์ตทันที (โปรดบันทึกงานของคุณและปิดเอกสารที่เปิดอยู่และอีเมลก่อน) หรือจัดเวลาการวินิจฉัยให้เรียกใช้โดยอัตโนมัติในครั้งถัดไปที่พีซีเริ่มระบบใหม่:</span><span class="sxs-lookup"><span data-stu-id="192d8-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![การวินิจฉัยหน่วยความจํา Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="192d8-109">เมื่อพีซีเริ่มระบบใหม่ เครื่องมือ **การวินิจฉัยหน่วยความจํา Windows** จะเรียกใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="192d8-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="192d8-110">สถานะและความคืบหน้าจะแสดงเป็นการเรียกใช้การวินิจฉัย และคุณจะมีตัวเลือกในการยกเลิกการวินิจฉัยโดยการกดแป้น **ESC** บนคีย์บอร์ดของคุณ</span><span class="sxs-lookup"><span data-stu-id="192d8-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="192d8-111">เมื่อการวินิจฉัยเสร็จสมบูรณ์ Windows จะเริ่มตามปกติ</span><span class="sxs-lookup"><span data-stu-id="192d8-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="192d8-112">หลังจากเริ่มระบบใหม่ทันที เมื่อเดสก์ท็อปปรากฏขึ้น การแจ้งเตือนจะปรากฏขึ้น (ถัดจากไอคอนศูนย์ปฏิบัติการบนแถบงาน) เพื่อระบุว่าพบข้อผิดพลาดของหน่วยความจําใดๆ หรือไม่</span><span class="sxs-lookup"><span data-stu-id="192d8-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="192d8-113">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="192d8-113">For example:</span></span>

<span data-ttu-id="192d8-114">ต่อไปนี้คือไอคอนศูนย์ปฏิบัติการ:</span><span class="sxs-lookup"><span data-stu-id="192d8-114">Here's the Action Center icon:</span></span> ![ไอคอนศูนย์ปฏิบัติการ](media/action-center-icon.png) 

<span data-ttu-id="192d8-116">และตัวอย่างการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="192d8-116">And a sample notification:</span></span> ![ไม่มีข้อผิดพลาดของหน่วยความจํา](media/no-memory-errors.png)

<span data-ttu-id="192d8-118">หากคุณไม่ได้รับการแจ้งเตือน คุณสามารถเลือก **ไอคอนศูนย์ปฏิบัติการ** บนแถบงานเพื่อแสดงรายการการแจ้งเตือนที่เลื่อนได้</span><span class="sxs-lookup"><span data-stu-id="192d8-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="192d8-119">เมื่อต้องการตรวจสอบข้อมูลโดยละเอียด **ให้พิมพ์** เหตุการณ์ลงในกล่องค้นหาบนแถบงานของคุณ แล้วเลือก **ตัวแสดง** เหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="192d8-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="192d8-120">ในบานหน้าต่าง **ด้านซ้ายของ** ตัวแสดงเหตุการณ์ ให้นําทางไปยัง แฟ้มบันทึก **ของ Windows > System**</span><span class="sxs-lookup"><span data-stu-id="192d8-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="192d8-121">ในบานหน้าต่างด้านขวามือ ให้สแกนรายการขณะที่ดูคอลัมน์ **แหล่งข้อมูล** จนกว่าคุณจะเห็นเหตุการณ์ด้วย ค่าแหล่งข้อมูล **MemoryDiagnostics-Results**</span><span class="sxs-lookup"><span data-stu-id="192d8-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="192d8-122">เน้นแต่ละเหตุการณ์ดังกล่าวและดูข้อมูลผลลัพธ์ในกล่องภายใต้ **แท็บ** ทั่วไป ทางด้านล่างของรายการ</span><span class="sxs-lookup"><span data-stu-id="192d8-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
