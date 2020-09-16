---
title: เรียกใช้การวินิจฉัยหน่วยความจำของ Windows ใน Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720809"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="1ca67-102">เรียกใช้การวินิจฉัยหน่วยความจำของ Windows ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="1ca67-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="1ca67-103">ถ้า Windows และแอปบนพีซีของคุณหยุดทำงานให้หยุดทำงานหรือทำงานในลักษณะที่ไม่เสถียรคุณอาจมีปัญหาเกี่ยวกับหน่วยความจำของพีซี (RAM)</span><span class="sxs-lookup"><span data-stu-id="1ca67-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="1ca67-104">คุณสามารถเรียกใช้การวินิจฉัยหน่วยความจำของ Windows เพื่อตรวจหาปัญหาเกี่ยวกับ RAM ของพีซีได้</span><span class="sxs-lookup"><span data-stu-id="1ca67-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="1ca67-105">ในกล่องค้นหาบนแถบงานของคุณให้พิมพ์การ**วินิจฉัยหน่วยความจำ**จากนั้นเลือก**Windows วินิจฉัยหน่วยความจำ**</span><span class="sxs-lookup"><span data-stu-id="1ca67-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="1ca67-106">เมื่อต้องการเรียกใช้การวิเคราะห์การเชื่อมต่อพีซีจำเป็นต้องเริ่มการทำงานใหม่</span><span class="sxs-lookup"><span data-stu-id="1ca67-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="1ca67-107">คุณมีตัวเลือกในการรีสตาร์ตทันที (โปรดบันทึกงานของคุณและปิดเอกสารและอีเมลที่เปิดอยู่ก่อน) หรือจัดกำหนดการการวินิจฉัยให้ทำงานโดยอัตโนมัติในครั้งถัดไปที่เริ่มระบบพีซีใหม่:</span><span class="sxs-lookup"><span data-stu-id="1ca67-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![การวินิจฉัยหน่วยความจำของ Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="1ca67-109">เมื่อเริ่มระบบพีซีใหม่เครื่อง **มือการวินิจฉัยหน่วยความจำของ Windows** จะทำงานโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1ca67-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="1ca67-110">สถานะและความคืบหน้าจะแสดงเป็นการเรียกใช้การวินิจฉัยและคุณมีตัวเลือกในการยกเลิกการวินิจฉัยโดยการกดปุ่ม **ESC** บนคีย์บอร์ดของคุณ</span><span class="sxs-lookup"><span data-stu-id="1ca67-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="1ca67-111">เมื่อการวินิจฉัยเสร็จสมบูรณ์แล้ว Windows จะเริ่มทำงานตามปกติ</span><span class="sxs-lookup"><span data-stu-id="1ca67-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="1ca67-112">ทันทีหลังจากเริ่มการทำงานใหม่เมื่อเดสก์ท็อปปรากฏขึ้นจะมีการแจ้งเตือนปรากฏขึ้น (ถัดจากไอคอน **ศูนย์ปฏิบัติ** การบนแถบงาน) เพื่อระบุว่าพบข้อผิดพลาดของหน่วยความจำหรือไม่</span><span class="sxs-lookup"><span data-stu-id="1ca67-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="1ca67-113">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="1ca67-113">For example:</span></span>

<span data-ttu-id="1ca67-114">นี่คือไอคอนศูนย์ปฏิบัติการ:</span><span class="sxs-lookup"><span data-stu-id="1ca67-114">Here's the Action Center icon:</span></span> ![ไอคอนศูนย์ปฏิบัติการ](media/action-center-icon.png) 

<span data-ttu-id="1ca67-116">และตัวอย่างการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="1ca67-116">And a sample notification:</span></span> ![ไม่มีข้อผิดพลาดของหน่วยความจำ](media/no-memory-errors.png)

<span data-ttu-id="1ca67-118">ถ้าคุณพลาดการแจ้งเตือนคุณสามารถเลือกไอคอน **ศูนย์ปฏิบัติการ** บนแถบงานเพื่อแสดง **ศูนย์ปฏิบัติ** การและดูรายการการแจ้งเตือนที่เลื่อนได้</span><span class="sxs-lookup"><span data-stu-id="1ca67-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="1ca67-119">เมื่อต้องการตรวจทานข้อมูลโดยละเอียดให้พิมพ์**เหตุการณ์**ลงในกล่องค้นหาบนแถบงานของคุณแล้วเลือก**ตัวแสดงเหตุการณ์**</span><span class="sxs-lookup"><span data-stu-id="1ca67-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="1ca67-120">ในบานหน้าต่างด้านซ้ายของ**ตัวแสดงเหตุการณ์**ให้นำทางไปยัง**ไฟล์บันทึกของ Windows > ระบบ**</span><span class="sxs-lookup"><span data-stu-id="1ca67-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="1ca67-121">ในบานหน้าต่างด้านขวาให้สแกนรายการในขณะที่ดูคอลัมน์**ต้นฉบับ**จนกว่าคุณจะเห็นเหตุการณ์ที่มีค่าแหล่งข้อมูล**MemoryDiagnostics-ผลลัพธ์**</span><span class="sxs-lookup"><span data-stu-id="1ca67-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="1ca67-122">เน้นเหตุการณ์ดังกล่าวแต่ละรายการและดูข้อมูลผลลัพธ์ในกล่องภายใต้แท็บ **ทั่วไป** ที่อยู่ด้านล่างรายการ</span><span class="sxs-lookup"><span data-stu-id="1ca67-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
