---
title: ดับเบิลคลิกไฟล์ Office เพื่อเปิดไม่สํานักงาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814824"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="5ed69-102">ดับเบิลคลิกไฟล์ Office เพื่อเปิดไม่สํานักงาน</span><span class="sxs-lookup"><span data-stu-id="5ed69-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="5ed69-103">หลังจากดับเบิลคลิกที่ไฟล์ Office คุณอาจเห็นโปรแกรมเปิดแต่ไฟล์ไม่เปิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="5ed69-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="5ed69-104">หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งสั่งไปยังโปรแกรม"</span><span class="sxs-lookup"><span data-stu-id="5ed69-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="5ed69-105">มีหลายสาเหตุดังนี้ แต่วิธีแก้ปัญหาที่พบบ่อยที่สุดสองวิธีคือ:</span><span class="sxs-lookup"><span data-stu-id="5ed69-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="5ed69-106">จากภายใน Excel ตรวจสอบให้แน่ใจว่าไม่ได้เลือกตัวเลือก DDE แล้ว</span><span class="sxs-lookup"><span data-stu-id="5ed69-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="5ed69-107">ตัวเลือกสามารถพบได้โดยการสร้างเวิร์กบุ๊กใหม่ แล้วเลือก ไฟล์ > บันทึก>**ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="5ed69-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="5ed69-108">ในส่วน **ทั่วไป** ให้ยกเลิกการเลือก **ละเว้นแอปพลิเคชันอื่นที่ใช้ Dynamic Data Exchange (DDE)**</span><span class="sxs-lookup"><span data-stu-id="5ed69-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="5ed69-109">เรียกใช้ การซ่อมแซมแบบออนไลน์ เพื่อคืนค่าการตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="5ed69-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="5ed69-110">คลิกปุ่ม เริ่ม ของ Windows แล้วค้นหา "แผงควบคุม"</span><span class="sxs-lookup"><span data-stu-id="5ed69-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="5ed69-111">เปิด **แผงควบคุม แล้ว** ไปที่ โปรแกรม **> และ** ฟีเจอร์</span><span class="sxs-lookup"><span data-stu-id="5ed69-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="5ed69-112">คลิกขวาที่ Microsoft **Office [เวอร์ชัน] แล้วเลือก** เปลี่ยน **>ซ่อมแซม** แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="5ed69-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="5ed69-113">ถ้าโซลูชันเหล่านี้ไม่ได้ผล คุณสามารถดูรายการโซลูชันทั้งหมดได้ในบทความสนับสนุน ดับเบิล [คลิกไฟล์ Office ล้มเหลวในการ](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)เปิด</span><span class="sxs-lookup"><span data-stu-id="5ed69-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
