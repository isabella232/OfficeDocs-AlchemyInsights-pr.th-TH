---
title: การคลิกสองครั้งที่แฟ้ม Office ล้มเหลวในการเปิด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573602"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="01c19-102">การคลิกสองครั้งที่แฟ้ม Office ล้มเหลวในการเปิด</span><span class="sxs-lookup"><span data-stu-id="01c19-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="01c19-103">หลังจากการคลิกสองครั้งที่แฟ้ม Office คุณอาจเห็นโปรแกรมเปิดแต่แฟ้มตัวเองไม่เปิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="01c19-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="01c19-104">หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งคำสั่งไปยังโปรแกรม"</span><span class="sxs-lookup"><span data-stu-id="01c19-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="01c19-105">มีสาเหตุมากมายสำหรับการนี้แต่สองวิธีการแก้ปัญหาที่พบบ่อยที่สุดคือ:</span><span class="sxs-lookup"><span data-stu-id="01c19-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="01c19-106">จากภายใน Excel ให้แน่ใจว่าตัวเลือก DDE จะถูกยกเลิก</span><span class="sxs-lookup"><span data-stu-id="01c19-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="01c19-107">ตัวเลือกที่สามารถพบได้โดยการสร้างสมุดงานใหม่แล้วเลือก**ตัวเลือก > แฟ้ม > ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="01c19-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="01c19-108">ในส่วน**ทั่วไป**ให้ยกเลิกการเลือก**ละเว้นโปรแกรมประยุกต์อื่นที่ใช้การแลกเปลี่ยนข้อมูลแบบไดนามิก (DDE)**</span><span class="sxs-lookup"><span data-stu-id="01c19-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="01c19-109">เรียกใช้การซ่อมแซมแบบออนไลน์เพื่อเรียกคืนการตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="01c19-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="01c19-110">คลิกที่ปุ่มเริ่มต้นของ Windows และค้นหา "แผงควบคุม"</span><span class="sxs-lookup"><span data-stu-id="01c19-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="01c19-111">เปิด**แผงควบคุม**และไปที่**โปรแกรม > โปรแกรมและคุณลักษณะ**</span><span class="sxs-lookup"><span data-stu-id="01c19-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="01c19-112">คลิกขวาที่**Microsoft Office [รุ่น]** แล้วเลือก**เปลี่ยน > ซ่อมแซมแบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="01c19-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="01c19-113">ถ้าไม่มีการแก้ไขปัญหาเหล่านี้จะพบรายการวิธีแก้ไขปัญหาที่สมบูรณ์มากขึ้นในบทความสนับสนุนการ[คลิกสองครั้งที่แฟ้ม Office ล้มเหลวในการเปิด](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="01c19-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
