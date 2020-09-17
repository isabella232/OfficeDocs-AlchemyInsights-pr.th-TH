---
title: การดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812098"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="f480a-102">การดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์</span><span class="sxs-lookup"><span data-stu-id="f480a-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="f480a-103">หลังจากดับเบิลคลิกที่ไฟล์ Office คุณอาจเห็นโปรแกรมเปิดแต่ไฟล์ตัวเองไม่เปิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="f480a-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="f480a-104">หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งคำสั่งไปยังโปรแกรม"</span><span class="sxs-lookup"><span data-stu-id="f480a-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="f480a-105">มีหลายสาเหตุสำหรับสิ่งนี้แต่มีวิธีแก้ไขปัญหาที่พบมากที่สุดสองวิธีดังนี้</span><span class="sxs-lookup"><span data-stu-id="f480a-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="f480a-106">จากภายใน Excel ให้ตรวจสอบให้แน่ใจว่าตัวเลือก DDE ไม่ได้ถูกยกเลิก</span><span class="sxs-lookup"><span data-stu-id="f480a-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="f480a-107">คุณสามารถค้นหาตัวเลือกได้โดยการสร้างเวิร์กบุ๊กใหม่แล้วเลือก**ตัวเลือก > ไฟล์ > ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="f480a-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="f480a-108">ในส่วน**ทั่วไป**ให้ยกเลิกการเลือก**ละเว้นแอปพลิเคชันอื่นที่ใช้การแลกเปลี่ยนข้อมูลแบบไดนามิก (DDE)**</span><span class="sxs-lookup"><span data-stu-id="f480a-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="f480a-109">เรียกใช้การซ่อมแซมแบบออนไลน์เพื่อคืนค่าการตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f480a-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="f480a-110">คลิกปุ่มเริ่มของ Windows และค้นหา "แผงควบคุม"</span><span class="sxs-lookup"><span data-stu-id="f480a-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="f480a-111">เปิด**แผงควบคุม**และไปที่**โปรแกรม > โปรแกรมและฟีเจอร์**</span><span class="sxs-lookup"><span data-stu-id="f480a-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="f480a-112">จากนั้นคลิกขวาที่**Microsoft Office [เวอร์ชัน]** แล้วเลือก**เปลี่ยน > การซ่อมแซมแบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="f480a-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="f480a-113">ถ้าไม่มีวิธีแก้ไขปัญหาเหล่านี้คุณสามารถดูรายการของโซลูชันที่สมบูรณ์มากขึ้นได้ในบทความสนับสนุนการ[ดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="f480a-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
