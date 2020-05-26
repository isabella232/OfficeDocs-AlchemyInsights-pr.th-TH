---
title: เรียกใช้การวินิจฉัยหน่วยความจําของ Windows ใน Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358292"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="5f65c-102">เรียกใช้การวินิจฉัยหน่วยความจําของ Windows ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="5f65c-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="5f65c-103">หาก Windows และแอปบนพีซีของคุณขัดข้อง การแช่แข็ง หรือการแสดงในลักษณะที่ไม่เสถียร คุณอาจมีปัญหากับหน่วยความจํา (RAM) ของพีซี</span><span class="sxs-lookup"><span data-stu-id="5f65c-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="5f65c-104">คุณสามารถเรียกใช้ Windows วินิจฉัยหน่วยความจําเพื่อตรวจสอบปัญหากับ RAM ของพีซี</span><span class="sxs-lookup"><span data-stu-id="5f65c-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="5f65c-105">ในกล่องค้นหาบนแถบงานของคุณ ให้พิมพ์**การวินิจฉัยหน่วยความจํา**แล้วเลือก**การวินิจฉัยหน่วยความจําของ Windows**</span><span class="sxs-lookup"><span data-stu-id="5f65c-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="5f65c-106">เมื่อต้องการเรียกใช้การวิเคราะห์การเชื่อมต่อ พีซีจําเป็นต้องเริ่มการทํางานใหม่</span><span class="sxs-lookup"><span data-stu-id="5f65c-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="5f65c-107">คุณมีตัวเลือกในการรีสตาร์ททันที (โปรดบันทึกงานและปิดเอกสารที่เปิดอยู่และอีเมลก่อน) หรือกําหนดการวินิจฉัยให้ทํางานโดยอัตโนมัติในครั้งต่อไปที่เครื่องคอมพิวเตอร์รีสตาร์ท:</span><span class="sxs-lookup"><span data-stu-id="5f65c-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![การวินิจฉัยหน่วยความจําของ Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="5f65c-109">เมื่อรีสตาร์ทเครื่องคอมพิวเตอร์ **, เครื่องมือวินิจฉัยหน่วยความจําของ Windows**จะทํางานโดยอัตโนมัติ.</span><span class="sxs-lookup"><span data-stu-id="5f65c-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="5f65c-110">สถานะและความคืบหน้าจะแสดงเป็นการเรียกใช้การวินิจฉัย และคุณมีตัวเลือกในการยกเลิกการวินิจฉัยโดยการกดปุ่ม**ESC**บนแป้นพิมพ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="5f65c-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="5f65c-111">เมื่อการวินิจฉัยเสร็จสมบูรณ์ Windows จะเริ่มต้นตามปกติ</span><span class="sxs-lookup"><span data-stu-id="5f65c-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="5f65c-112">ทันทีหลังจากรีสตาร์ทเมื่อ Desktop ปรากฏขึ้นการแจ้งเตือนจะปรากฏขึ้น (ถัดจากไอคอน**ศูนย์ปฏิบัติการ**บนแถบงาน) เพื่อบ่งชี้ว่าพบข้อผิดพลาดของหน่วยความจํา</span><span class="sxs-lookup"><span data-stu-id="5f65c-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="5f65c-113">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="5f65c-113">For example:</span></span>

<span data-ttu-id="5f65c-114">นี่คือไอคอน 'ศูนย์ปฏิบัติการ'</span><span class="sxs-lookup"><span data-stu-id="5f65c-114">Here's the Action Center icon:</span></span> ![ไอคอนศูนย์ปฏิบัติการ](media/action-center-icon.png) 

<span data-ttu-id="5f65c-116">และตัวอย่างการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="5f65c-116">And a sample notification:</span></span> ![ไม่มีข้อผิดพลาดหน่วยความจํา](media/no-memory-errors.png)

<span data-ttu-id="5f65c-118">ถ้าคุณพลาดการแจ้งเตือน คุณสามารถเลือกไอคอน **'ศูนย์ปฏิบัติการ**' บนแถบงานเพื่อแสดง **'ศูนย์ปฏิบัติการ'** และดูรายการการแจ้งเตือนที่เลื่อนได้</span><span class="sxs-lookup"><span data-stu-id="5f65c-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="5f65c-119">เมื่อต้องการตรวจทานข้อมูลโดยละเอียด ให้พิมพ์**เหตุการณ์**ลงในกล่องค้นหาบนแถบงานของคุณ แล้วเลือก**ตัวแสดงเหตุการณ์**</span><span class="sxs-lookup"><span data-stu-id="5f65c-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="5f65c-120">ในบานหน้าต่างด้านซ้ายของ**ตัวแสดงเหตุการณ์**นําทางไปยัง**Windows Logs > ระบบ**</span><span class="sxs-lookup"><span data-stu-id="5f65c-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="5f65c-121">ในบานหน้าต่างด้านขวา ให้สแกนรายการลงในขณะที่กําลังค้นหาที่คอลัมน์ **'แหล่ง**' จนกว่าคุณจะเห็นเหตุการณ์ที่มีค่า**Source MemoryDiagnostics-Results**</span><span class="sxs-lookup"><span data-stu-id="5f65c-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="5f65c-122">เน้นเหตุการณ์ดังกล่าวและดูข้อมูลผลลัพธ์ในกล่องภายใต้แท็บ**ทั่วไป**ใต้รายการ</span><span class="sxs-lookup"><span data-stu-id="5f65c-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
